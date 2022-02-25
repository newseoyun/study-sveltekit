<script lang="ts">
    import TopAppBar, { Row, Section, Title } from '@smui/top-app-bar';
    import IconButton from '@smui/icon-button';
    export let title = "스벨트 하이"
</script>

<div class="title">
    <TopAppBar
    variant="static"
    color='primary'
  >
    <Row>
      <Section>
        <IconButton class="material-icons">menu</IconButton>
        <Title>{title}</Title>
      </Section>
      <Section align="end" toolbar>
        <IconButton class="material-icons" aria-label="Download"
          >file_download</IconButton
        >
        <IconButton class="material-icons" aria-label="Print this page"
          >print</IconButton
        >
        <IconButton class="material-icons" aria-label="Bookmark this page"
          >bookmark</IconButton
        >
      </Section>
    </Row>
  </TopAppBar>
</div>

<style>
    /* your styles go here */
</style>