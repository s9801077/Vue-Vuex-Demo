<template>
  <div>
    <NavBar>
      <div slot="right">
        <input class="form-control mr-sm-2" type="text" placeholder="Account" aria-label="Account">
        <input class="form-control mr-sm-2" type="password" placeholder="Password" aria-label="Password">
        <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Login</button>
      </div>
    </NavBar>
    <JumBotron></JumBotron>
    <Container :list="list"></Container>
  </div>
</template>
<script>
  import NavBar from '../components/navbar'
  import JumBotron from '../components/jumbotron'
  import Container from '../components/container'

  export default {
    name: 'learnComponent',
    data() {
      return {
        list: [
          {
            title: 'Heading 1',
            info: 'Donec id elit non mi porta gravida at eget metus. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Etiam porta sem malesuada magna mollis euismod. Donec sed odio dui. ',
            btntext: 'View details »'
          },
          {
            title: 'Heading 2',
            info: 'Donec id elit non mi porta gravida at eget metus. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Etiam porta sem malesuada magna mollis euismod. Donec sed odio dui. ',
            btntext: 'View details »'
          },
          {
            title: 'Heading 3',
            info: 'Donec sed odio dui. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Vestibulum id ligula porta felis euismod semper. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.',
            btntext: 'View details »'
          },
        ]
      }
    },
    components: {
      NavBar,
      JumBotron,
      Container,
    },
  }
</script>
