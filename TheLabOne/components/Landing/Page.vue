<template>
  <div>
    <LandingHeroSection
      :imgHero="imgHero"
      :title="titleHero"
      :description="descriptionHero"
      :imgHeroShadow="imgHeroShadow"
      :imgHeroRounded="imgHeroRounded"
      :imgHeroPosition="imgHeroPosition"
      :imgHeroFit="imgHeroFit"
      :imgHeroWidth="imgHeroWidth"
      :imgHeroHeight="imgHeroHeight"
      :color="color"
      :appName="appName"
    />
    <LandingAdvantages
      :color="color"
      :advantages="advantages"
      :appName="appName"
    />
    <LandingHowItsWorks
      :imgArg="imgArg"
      :imgArgShadow="imgArgShadow"
      :imgArgRounded="imgArgRounded"
      :imgArgPosition="imgArgPosition"
      :imgArgFit="imgArgFit"
      :imgArgWidth="imgArgWidth"
      :imgArgHeight="imgArgHeight"
    />
    <LandingPricing
      :color="color"
      :pricing="pricing"
    />
    <LandingTestimonials
      :testimonials="testimonials"
    />
    <LandingGetEmail
      :color="color"
    />
  </div>
</template>

<script>
export default {
  name: "Page",
  data() {
    return {
      titleHero: "The Lab One",
      descriptionHero: "Nous avons la solution pour vos solutions web 🪄",
      color: "bg-blue-300",
      imgHero: "https://cuansjfifujgnuwfznsx.supabase.co/storage/v1/object/public/landing-generator-bucket/images/1_1732812241721_heroImage.jpeg",
      imgArg: null,
      imgHeroShadow: true,
      imgHeroRounded: true,
      imgArgShadow: false,
      imgArgRounded: false,
      imgHeroPosition: "top",
      imgHeroFit: "cover",
      imgHeroWidth: "81",
      imgHeroHeight: "85",
      imgArgPosition: "center",
      imgArgFit: "contain",
      imgArgWidth: "50",
      imgArgHeight: "50",
      advantages: [{"title":"Sur mesure ","text":"Une solution conçu sur mesure pour correspondre à 100% à vos besoins "},{"title":"Délais imbattables ","text":"Nos équipes s’occupent de vous dans un délai battant toute concurrence "},{"title":"Taris imbattables","text":"Des tarifs adaptés à vos besoins défiants toute concurrence "}],
      testimonials: [],
      pricing: [{"title":"Site vitrine","price":300,"duration":"site","features":["Une page optimisé et référencée","Vos avis Google mis en avant","Taux de conversion optimisé"]},{"title":"E-commerce","price":600,"duration":"à partir de ","features":["Paiement intégré","Plateforme de gestion de vos produits","Optimisé et référencé"]},{"title":"Autre demande","price":"","duration":"nous contacter","features":["Toute vos solutions sur demande"]}],
      appName: "The Lab One",
    };
  },
};
</script>