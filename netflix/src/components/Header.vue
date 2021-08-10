<script>
import { ref } from "vue";
export default {
  setup() {
    const navLinks = ref({
      Home: {
        name: "Home",
        href: "/"
      },
      TvShows: {
        name: "Shows",
        href: "/about"
      },
      Series: {
        name: "Series",
        href: "#"
      }
    });
    return { navLinks };
  }
};
</script>