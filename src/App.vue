<script lang="ts">
  import Main from "./components/layout/Main.vue";

  export default {
    components: {
      Main,
    },
  }
</script>

<template>
    
    <Main>

        <h1 class="text-5xl mb-10">Инвестируй в твердую волюту онлайн</h1>

        <input type="text" name="" id="amount-of-money" placeholder="Введите сумму"
               class="block py-4 px-8 text-2xl border-pink-500"
               pattern="[0-9]{3}\s[0-9]{3}\s[0-9]{3}\s+(\.\d{2})?">

        <label for="amount-of-money">Укажите сумму рублей, которую собираетесь продать</label>

        <table>
          <tr>
            <td></td>
            <td></td>
            <td></td>
          </tr>
          <tr>
            <td></td>
            <td></td>
            <td></td>
          </tr>
          <tr>
            <td></td>
            <td></td>
            <td></td>
          </tr>
          <tr>
            <td></td>
            <td></td>
            <td></td>
          </tr>
          <tr>
            <td></td>
            <td></td>
            <td></td>
          </tr>
        </table>

    </Main>

</template>
