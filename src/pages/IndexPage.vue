<template>
  <q-page class=" ">
    
    <q-carousel
      swipeable
      animated
      v-model="slide"
      :autoplay="autoplay"
      ref="carousel"
      infinite
    >
      <q-carousel-slide :name="1" img-src="https://www.daysoftheyear.com/wp-content/uploads/national-fast-food-day.jpg" />
      <q-carousel-slide :name="2" img-src="https://www.mashed.com/img/gallery/the-best-new-fast-food-menu-items-weve-tried-in-2023-so-far/intro-1682446897.jpg" />
      <q-carousel-slide :name="3" img-src="https://www.tastingtable.com/img/gallery/12-low-carb-fast-food-options-that-wont-ruin-your-diet/intro-1651501665.jpg" />
      <q-carousel-slide :name="4" img-src="https://cdn.firstcry.com/education/2022/11/12144827/List-of-Fast-Food-Fast-Food-Vocabulary-for-Kids.jpg" />

      <template v-slot:control>
        <q-carousel-control
          position="top-right"
          :offset="[18, 18]"
          class="text-white rounded-borders"
          style="background: rgba(0, 0, 0, .3); padding: 4px 8px;"
        >
          <q-toggle dense dark color="orange" v-model="autoplay" label="Auto Play" />
        </q-carousel-control>

        <q-carousel-control
          position="bottom-right"
          :offset="[18, 18]"
          class="q-gutter-xs"
        >
          <q-btn
            push round dense color="orange" text-color="black" icon="arrow_left"
            @click="$refs.carousel.previous()"
          />
          <q-btn
            push round dense color="orange" text-color="black" icon="arrow_right"
            @click="$refs.carousel.next()"
          />
        </q-carousel-control>
      </template>
    </q-carousel>
<div class="row item-start q-gutter-md q-pa-md">
  <div class="col">
    <q-card class="my-card" flat bordered>
  <q-img src="https://cdn.quasar.dev/img/chicken-salad.jpg" />

  <q-card-section>
    <q-btn
      fab
      color="primary"
      icon="place"
      class="absolute"
      style="top: 0; right: 12px; transform: translateY(-50%);"
    />

    <div class="row no-wrap items-center">
      <div class="col text-h6 ellipsis">
        Cafe 1
      </div>
      <div class="col-auto text-grey text-caption q-pt-md row no-wrap items-center">
        <q-icon name="place" />
        250 ft
      </div>
    </div>

    <q-rating v-model="stars" :max="5" size="32px" />
  </q-card-section>

  <q-card-section class="q-pt-none">
    <div class="text-subtitle1">
      $・Sri lanka, Cafe
    </div>
    <div class="text-caption text-grey">
      Small plates, salads & sandwiches in an intimate setting.
    </div>
  </q-card-section>

  <q-separator />

  <q-card-actions>
    <q-btn flat round icon="event" />
    <q-btn flat color="primary">
      Reserve
    </q-btn>
  </q-card-actions>
</q-card>
</div>
<div class="col">
    <q-card class="my-card" flat bordered>
  <q-img src="https://cdn.quasar.dev/img/chicken-salad.jpg" />

  <q-card-section>
    <q-btn
      fab
      color="primary"
      icon="place"
      class="absolute"
      style="top: 0; right: 12px; transform: translateY(-50%);"
    />

    <div class="row no-wrap items-center">
      <div class="col text-h6 ellipsis">
        Cafe 2
      </div>
      <div class="col-auto text-grey text-caption q-pt-md row no-wrap items-center">
        <q-icon name="place" />
        250 ft
      </div>
    </div>

    <q-rating v-model="stars" :max="5" size="32px" />
  </q-card-section>

  <q-card-section class="q-pt-none">
    <div class="text-subtitle1">
      $・Sri lanka, Cafe
    </div>
    <div class="text-caption text-grey">
      Small plates, salads & sandwiches in an intimate setting.
    </div>
  </q-card-section>

  <q-separator />

  <q-card-actions>
    <q-btn flat round icon="event" />
    <q-btn flat color="primary">
      Reserve
    </q-btn>
  </q-card-actions>
</q-card>
</div>
<div class="col">
    <q-card class="my-card" flat bordered>
  <q-img src="https://cdn.quasar.dev/img/chicken-salad.jpg" />

  <q-card-section>
    <q-btn
      fab
      color="primary"
      icon="place"
      class="absolute"
      style="top: 0; right: 12px; transform: translateY(-50%);"
    />

    <div class="row no-wrap items-center">
      <div class="col text-h6 ellipsis">
        Cafe 3
      </div>
      <div class="col-auto text-grey text-caption q-pt-md row no-wrap items-center">
        <q-icon name="place" />
        250 ft
      </div>
    </div>

    <q-rating v-model="stars" :max="5" size="32px" />
  </q-card-section>

  <q-card-section class="q-pt-none">
    <div class="text-subtitle1">
      $・Sri lanka, Cafe
    </div>
    <div class="text-caption text-grey">
      Small plates, salads & sandwiches in an intimate setting.
    </div>
  </q-card-section>

  <q-separator />

  <q-card-actions>
    <q-btn flat round icon="event" />
    <q-btn flat color="primary">
      Reserve
    </q-btn>
  </q-card-actions>
</q-card>
</div>
<div class="col">
    <q-card class="my-card" flat bordered>
  <q-img src="https://cdn.quasar.dev/img/chicken-salad.jpg" />

  <q-card-section>
    <q-btn
      fab
      color="primary"
      icon="place"
      class="absolute"
      style="top: 0; right: 12px; transform: translateY(-50%);"
    />

    <div class="row no-wrap items-center">
      <div class="col text-h6 ellipsis">
        Cafe 4
      </div>
      <div class="col-auto text-grey text-caption q-pt-md row no-wrap items-center">
        <q-icon name="place" />
        250 ft
      </div>
    </div>

    <q-rating v-model="stars" :max="5" size="32px" />
  </q-card-section>

  <q-card-section class="q-pt-none">
    <div class="text-subtitle1">
      $・Sri lanka, Cafe
    </div>
    <div class="text-caption text-grey">
      Small plates, salads & sandwiches in an intimate setting.
    </div>
  </q-card-section>

  <q-separator />

  <q-card-actions>
    <q-btn flat round icon="event" />
    <q-btn flat color="primary">
      Reserve
    </q-btn>
  </q-card-actions>
</q-card>
</div>
</div>

<div class="row item-start q-gutter-md">
  <div class="col">
    <q-card class="my-card" flat bordered>
  <q-img src="https://cdn.quasar.dev/img/chicken-salad.jpg" />

  <q-card-section>
    <q-btn
      fab
      color="primary"
      icon="place"
      class="absolute"
      style="top: 0; right: 12px; transform: translateY(-50%);"
    />

    <div class="row no-wrap items-center">
      <div class="col text-h6 ellipsis">
        Cafe 5
      </div>
      <div class="col-auto text-grey text-caption q-pt-md row no-wrap items-center">
        <q-icon name="place" />
        250 ft
      </div>
    </div>

    <q-rating v-model="stars" :max="5" size="32px" />
  </q-card-section>

  <q-card-section class="q-pt-none">
    <div class="text-subtitle1">
      $・Sri lanka, Cafe
    </div>
    <div class="text-caption text-grey">
      Small plates, salads & sandwiches in an intimate setting.
    </div>
  </q-card-section>

  <q-separator />

  <q-card-actions>
    <q-btn flat round icon="event" />
    <q-btn flat color="primary">
      Reserve
    </q-btn>
  </q-card-actions>
</q-card>
</div>
<div class="col">
    <q-card class="my-card" flat bordered>
  <q-img src="https://cdn.quasar.dev/img/chicken-salad.jpg" />

  <q-card-section>
    <q-btn
      fab
      color="primary"
      icon="place"
      class="absolute"
      style="top: 0; right: 12px; transform: translateY(-50%);"
    />

    <div class="row no-wrap items-center">
      <div class="col text-h6 ellipsis">
        Cafe 6
      </div>
      <div class="col-auto text-grey text-caption q-pt-md row no-wrap items-center">
        <q-icon name="place" />
        250 ft
      </div>
    </div>

    <q-rating v-model="stars" :max="5" size="32px" />
  </q-card-section>

  <q-card-section class="q-pt-none">
    <div class="text-subtitle1">
      $・Sri lanka, Cafe
    </div>
    <div class="text-caption text-grey">
      Small plates, salads & sandwiches in an intimate setting.
    </div>
  </q-card-section>

  <q-separator />

  <q-card-actions>
    <q-btn flat round icon="event" />
    <q-btn flat color="primary">
      Reserve
    </q-btn>
  </q-card-actions>
</q-card>
</div>
<div class="col">
    <q-card class="my-card" flat bordered>
  <q-img src="https://cdn.quasar.dev/img/chicken-salad.jpg" />

  <q-card-section>
    <q-btn
      fab
      color="primary"
      icon="place"
      class="absolute"
      style="top: 0; right: 12px; transform: translateY(-50%);"
    />

    <div class="row no-wrap items-center">
      <div class="col text-h6 ellipsis">
        Cafe 7
      </div>
      <div class="col-auto text-grey text-caption q-pt-md row no-wrap items-center">
        <q-icon name="place" />
        250 ft
      </div>
    </div>

    <q-rating v-model="stars" :max="5" size="32px" />
  </q-card-section>

  <q-card-section class="q-pt-none">
    <div class="text-subtitle1">
      $・Sri lanka, Cafe
    </div>
    <div class="text-caption text-grey">
      Small plates, salads & sandwiches in an intimate setting.
    </div>
  </q-card-section>

  <q-separator />

  <q-card-actions>
    <q-btn flat round icon="event" />
    <q-btn flat color="primary">
      Reserve
    </q-btn>
  </q-card-actions>
</q-card>
</div>
<div class="col">
    <q-card class="my-card" flat bordered>
  <q-img src="https://cdn.quasar.dev/img/chicken-salad.jpg" />

  <q-card-section>
    <q-btn
      fab
      color="primary"
      icon="place"
      class="absolute"
      style="top: 0; right: 12px; transform: translateY(-50%);"
    />

    <div class="row no-wrap items-center">
      <div class="col text-h6 ellipsis">
        Cafe 8
      </div>
      <div class="col-auto text-grey text-caption q-pt-md row no-wrap items-center">
        <q-icon name="place" />
        250 ft
      </div>
    </div>

    <q-rating v-model="stars" :max="5" size="32px" />
  </q-card-section>

  <q-card-section class="q-pt-none">
    <div class="text-subtitle1">
      $・Sri lanka, Cafe
    </div>
    <div class="text-caption text-grey">
      Small plates, salads & sandwiches in an intimate setting.
    </div>
  </q-card-section>

  <q-separator />

  <q-card-actions>
    <q-btn flat round icon="event" />
    <q-btn flat color="primary">
      Reserve
    </q-btn>
  </q-card-actions>
</q-card>
</div>
</div>

  </q-page>
</template>

<script>
import { defineComponent } from 'vue'
import { ref } from 'vue'

export default defineComponent({
  name: 'IndexPage',
  setup () {
    return {
      slide: ref(1),
      autoplay: ref(false)
    }
  }
})
</script>
