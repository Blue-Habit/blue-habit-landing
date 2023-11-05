<template>
  <div class="teams mx-auto pb-9 bg-gray-100">
    <h1 class="text-primary text-xl lg:px-16 sm:px-5">Our Teams</h1>
    <div class="grid lg:grid-cols-2 sm:grid-cols-1">
      <h1 class="text-5xl text-gray-900 font-bold pt-3 lg:px-16 sm:px-5">
        Exceptional and <br />
        trusty challengers
      </h1>
      <div class="block lg:pr-16 sm:px-5">
        <p class="text-gray-700 pb-3">
          We firmly believe that there's no path to success where we stand alone
          on an island. It's together that we flourish and achieve greatness.
        </p>
        <button
          class="bg-primary hover:bg-primary-dark py-2 px-3 text-white rounded"
        >
          About Us
        </button>
      </div>
    </div>
  </div>
  <div
    class="grid lg:grid-cols-3 sm:grid-cols-1 lg:px-16 sm:px-5 gap-7 pt-5 bg-gray-100"
  >
    <CardTeams
      v-for="teamMember in teamMembers"
      :key="teamMember.id"
      :name="teamMember.name"
      :position="teamMember.position"
      :imageSrc="teamMember.imageSrc"
      :linkedinUrl="teamMember.linkedinUrl"
    />
  </div>
</template>

<script>
import CardTeams from "./CardTeams";
import imgMario from "@/assets/img/img-mario.png";
import imgTrian from "@/assets/img/img-trian.png";
import imgFirman from "@/assets/img/img-firman.png";
import imgSusilo from "@/assets/img/img-susilo.png";
import imgHerry from "@/assets/img/img-herry.png";
import imgWahyu from "@/assets/img/img-wahyu.png";

export default {
  name: "Teams",
  components: {
    CardTeams,
  },
  data() {
    return {
      teamMembers: [
        {
          id: 1,
          name: "Mario Prasetyo",
          position: "CEO",
          imageSrc: imgMario,
          linkedinUrl: "#",
        },
        {
          id: 2,
          name: "Trian Damai",
          position: "CTO",
          imageSrc: imgTrian,
          linkedinUrl: "#",
        },
        {
          id: 3,
          name: "Firman Hanafi",
          position: "CFO",
          imageSrc: imgFirman,
          linkedinUrl: "#",
        },
        {
          id: 4,
          name: "Susilo Setyabudi",
          position: "COO",
          imageSrc: imgSusilo,
          linkedinUrl: "#",
        },
        {
          id: 5,
          name: "Herry Susanto",
          position: "Product Manager",
          imageSrc: imgHerry,
          linkedinUrl: "#",
        },
        {
          id: 6,
          name: "Wahyu Renaldi",
          position: "Head of IT",
          imageSrc: imgWahyu,
          linkedinUrl: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped></style>
