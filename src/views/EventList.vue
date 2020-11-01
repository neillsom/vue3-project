<template>
  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
import EventCard from "@/components/EventCard.vue";

export default {
  name: "EventList",
  components: {
    EventCard,
  },
  data() {
    return {
      events: [
        {
          id: 274210136,
          category: "outdoors-adventure",
          title:
            "Learn about Environment Texas's efforts to reduce illegal air pollution",
          description:
            "Please join The Dallas Sierra Club in welcoming Environment Texas Clean Air Consultant, Catherine Fraser, as she details her work with leading clean air campaigns and reducing illegal air pollution from industrial facilities across Texas.",
          location: "Online event",
          date: "Tuesday, November 10, 2020",
          time: "7:00 PM CST",
          petsAllowed: true,
          organizer: "Kirk M.",
        },
        {
          id: 273692325,
          category: "outdoors-adventure",
          title: "Virtual pep rally: Texas A&M vs. LSU",
          description:
            "Join us for a virtual pep rally preceding the texas A&M-LSU game. This is going to be the one pep rally that decides who will be the meetup group member who is worthy of the title of “guardian of sports season”. Can you dig it?",
          location: "Online event",
          date: "Saturday, November 28, 2020",
          time: "12:00 PM CST",
          petsAllowed: true,
          organizer: "Jacob L.",
        },
        {
          id: 274232838,
          category: "outdoors-adventure",
          title: "Sober Cycling",
          description:
            "Come join us for some paved trails around White Rock Lake on Sunday November 1st at 9am. Bikes are limited, contact[masked] to reserve one.",
          location: "White Rock Paddle Co. 389 East Lawther Dr, Dallas, TX",
          date: "Sunday, November 1, 2020",
          time: "9:00 AM CST",
          petsAllowed: false,
          organizer: "Erin",
        },
        {
          id: 274224416,
          category: "outdoors-adventure",
          title: "Cottonwood Creek Clean Up",
          description:
            "Cottonwood Creek is rarely paddled and often trashed. Come join us on the water as we paddle this creek and help the environment. This event is jointly sponsored by North Texas River Runners, Trinity Coalition and Grand Prairie Adopt-A-Stream.",
          location: "Southeast 14th Street SE 14th St, Grand Prairie, TX",
          date: "Saturday, November 7, 2020",
          time: "8:00 AM CST",
          petsAllowed: false,
          organizer: "Teresa",
        },
      ],
    };
  },
};
</script>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>