<script>
  import TopAppBar, { Row, Section, Title } from '@smui/top-app-bar'
  import IconButton from '@smui/icon-button'

  import Drawer from './Drawer.svelte'

  export let title = '스벨트 하이'

  let open = false

  function toggleOpen() {
    open = !open
  }
</script>

<div class="title">
  <TopAppBar variant="static" color="primary">
    <Row>
      <Section>
        <IconButton class="material-icons" on:click={toggleOpen}>menu</IconButton>
        <Title>{title}</Title>
      </Section>
      <Section align="end" toolbar>
        <IconButton class="material-icons" aria-label="Download">file_download</IconButton>
        <IconButton class="material-icons" aria-label="Print this page">print</IconButton>
        <IconButton class="material-icons" aria-label="Bookmark this page">bookmark</IconButton>
      </Section>
    </Row>
  </TopAppBar>

  <Drawer bind:open />
</div>

<style>
  /* your styles go here */
</style>
