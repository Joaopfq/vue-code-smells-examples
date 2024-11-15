<script>

import { ref } from 'vue';

export default {
  setup() {
    const user = ref({
      name: 'João',
      address: {
        city: 'Quixadá',
        state: 'CE',
      },
    });

    function updateCity() {
      user.value.address.city = 'Fortaleza'; // Vue não detecta essa mudança
    }

    return {
      user,
      updateCity,
    };
  },
};

</script>