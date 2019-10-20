
<h1>Cocktails</h1>
<ul>
  {#each cocktails as cocktail}
    <li>{cocktail.title} ({cocktail.id})</li>
  {/each}
</ul>

<script>
  import axios from 'axios';
  export let cocktails = [];

  // Make a request for a user with a given ID
  // axios.get('localhost:3000/cocktails?id=1')
  //   .then(function (response) {
  //     // handle success
  //     console.log(response);
  //   })
  //   .catch(function (error) {
  //     // handle error
  //     console.log(error);
  //   })
  //   .finally(function () {
  //     // always executed
  //   });
  setTimeout(()=> {
    cocktails = [
      {
        id: 1,
        title: "Mojito",
        author: "thomas"
      },{
        id: 2,
        title: "klasd",
        author: "thomas"
      },{
        id: 3,
        title: "Negroni",
        author: "thomas"
      },
    ];
  }, 1000);
</script>
