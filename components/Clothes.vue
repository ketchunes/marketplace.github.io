<template>
  <div class="px-10 py-5 md:px-32">
    <div>
      <div id="woman" class="text-3xl mt-4 mb-12">Женщинам</div>
      <div class="grid md:grid-cols-2 xl:grid-cols-4 gap-10 mt-3">
        <div v-for="elem in lol" class="h-full flex flex-col gap-2">
          <div><img class="w-full" :src="elem.img" alt="" /></div>
          <div class="text-lg">{{ elem.title }}</div>
          <div>Коллекция 2023-2024</div>
          <div class="text-secondary-content mb-auto">{{ elem.price }}</div>
          <button class="active:scale-95 rounded-md hover:cursor-pointer w-fit transition">
            <CardHover
              border-radius="var(--radius-box)"
              container-color="var(--color-base-200)"
              light-color="var(--color-secondary-content)"
              base-color="var(--color-base-200)">
              <div class="py-2 px-4 font-semibold text-sm">ДОБАВИТЬ В КОРЗИНУ</div>
            </CardHover>
          </button>
        </div>
      </div>
      <div id="man" class="text-3xl mb-12 mt-20">Мужчинам</div>
      <div class="grid md:grid-cols-2 xl:grid-cols-4 gap-10 mt-3">
        <div v-for="elem in kek" class="h-full flex flex-col gap-2">
          <div><img class="w-full" :src="elem.img" alt="" /></div>
          <div class="text-lg">{{ elem.title }}</div>
          <div>Коллекция 2023-2024</div>
          <div class="text-secondary-content mb-auto">{{ elem.price }}</div>
          <button class="active:scale-95 rounded-md hover:cursor-pointer w-fit transition">
            <CardHover
              border-radius="var(--radius-box)"
              container-color="var(--color-base-200)"
              light-color="var(--color-secondary-content)"
              base-color="var(--color-base-200)">
              <div class="py-2 px-4 font-semibold text-sm">ДОБАВИТЬ В КОРЗИНУ</div>
            </CardHover>
          </button>
        </div>
      </div>
      <div id="all" class="text-3xl mb-12 mt-20">Распродажа</div>
      <div class="grid md:grid-cols-2 xl:grid-cols-4 gap-10 mt-3">
        <div v-for="elem in pelmeni" class="h-full flex flex-col gap-2">
          <div><img class="w-full" :src="elem.img" alt="" /></div>
          <div class="text-lg">{{ elem.title }}</div>
          <div>Коллекция 2023-2024</div>
          <div class="text-secondary-content mb-auto">{{ elem.price }}</div>
          <button class="active:scale-95 rounded-md hover:cursor-pointer w-fit transition">
            <CardHover
              border-radius="var(--radius-box)"
              container-color="var(--color-base-200)"
              light-color="var(--color-secondary-content)"
              base-color="var(--color-base-200)">
              <div class="py-2 px-4 font-semibold text-sm">ДОБАВИТЬ В КОРЗИНУ</div>
            </CardHover>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
  const lol = [
    {
      img: "img/cl-2.png",
      title: "ПАРКА ЗИМНЯЯ ЖЕНСКАЯ «МАРИИНКА»",
      subTitle: "Коллекция 2023-2024",
      price: "35.000 Тг.",
    },
    {
      img: "img/cl-1.png",
      title: "ПАРКА ЗИМНЯЯ ЖЕНСКАЯ «МАРИИНКА» ФУКСИЯ",
      subTitle: "Коллекция 2023-2024",
      price: "30.000 Тг.",
    },
    {
      img: "img/cl-3.png",
      title: "ПАРКА ЗИМНЯЯ ЖЕНСКАЯ «МАРИИНКА» ПЕРЛАМУТР",
      subTitle: "Коллекция 2023-2024",
      price: "38.000 Тг.",
    },
    {
      img: "img/cl-4.png",
      title: "КУРТКА КОРОТКАЯ ЗИМНЯЯ ЖЕНСКАЯ «ФОНТАНКА» БЕЖЕВАЯ",
      subTitle: "Коллекция 2023-2024",
      price: "35.000 Тг.",
    },
  ];

  const kek = [
    {
      img: "img/man-1.png",
      title: "ПАРКА ЗИМНЯЯ МУЖСКАЯ «АДМИРАЛТЕЙСТВО» ЧЁРНАЯ",
      subTitle: "Коллекция 2023-2024",
      price: "31.000 Тг.",
    },
    {
      img: "img/man-2.png",
      title: "КУРТКА КОРОТКАЯ МУЖСКАЯ «ВЕРФЬ» БЕЖЕВАЯ",
      subTitle: "Коллекция 2023-2024",
      price: "26.400 Тг.",
    },
    {
      img: "img/man-3.png",
      title: "ВЕТРОВКА МУЖСКАЯ ЧЁРНАЯ",
      subTitle: "Коллекция 2023-2024",
      price: "12.000 Тг.",
    },
    {
      img: "img/man-4.png",
      title: "ПЛАЩ МУЖСКОЙ DEEP BLUE",
      subTitle: "Коллекция 2023-2024",
      price: "17.500 Тг.",
    },
  ];

  const pelmeni = [
    {
      img: "img/woman-1.png",
      title: "ПАЛЬТО ТЁПЛОЕ ЖЕНСКОЕ «ЭРМИТАЖ» МЯТНОЕ",
      subTitle: "Коллекция 2023-2024",
      price: "17.500 Тг.",
    },
    {
      img: "img/woman-2.png",
      title: "ПАЛЬТО ТЁПЛОЕ ЖЕНСКОЕ «ЭРМИТАЖ» ОРХИДЕЯ",
      subTitle: "Коллекция 2023-2024",
      price: "14.000 Тг.",
    },
    {
      img: "img/woman-3.png",
      title: "ПАЛЬТО ТЁПЛОЕ ЖЕНСКОЕ «ЭРМИТАЖ» ЧЁРНОЕ",
      subTitle: "Коллекция 2023-2024",
      price: "19.600 Тг.",
    },
    {
      img: "img/woman-4.png",
      title: "ПАЛЬТО ТЁПЛОЕ ЖЕНСКОЕ ПЫЛЬНО-ГОЛУБОЕ",
      subTitle: "Коллекция 2023-2024",
      price: "15.400 Тг.",
    },
  ];
</script>
