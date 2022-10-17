<template>
  <main>
    <div class="container">
      <section>
        <img
          srcset="
            https://www.ionos.com/digitalguide/fileadmin/_processed_/2/d/csm_sitemap-t_f89576c988.jpg
          "
          class="leftimg"
        />
        <p>
          The Document Object Model, DOM for short, is a standardized
          programming interface for the structuring of HTML and XML documents.
          It was developed and released by the World Wide Consortium (W3C), the
          organization founded by web inventor Tim Berners-Lee in 1994, to
          design and establish standards for the World Wide Web. The purpose of
          the Document Object Model is to make it as easy as possible for
          programmers to access a web project’s components so that they can add
          to, delete and edit the project’s content, attributes, and styles. DOM
          serves as a platform-independent and language-neutral link between
          script languages such as JavaScript and the basic web document, as it
          depicts the structure of the document in a tree structure in which
          every node is an independent, selectable object. Because of this
          structure, one also refers to this type of displayed web project
          version as a DOM tree.
        </p>
      </section>

      <section>
        <h3>API</h3>

        <ol>
          <li>const linkRef = document.querySelector(NODE);</li>
          <li>let child = Document.createElement(NODE);</li>
          <li>linkRef.appendChild(child)</li>
        </ol>
      </section>
    </div>
  </main>
</template>

<script>
export default {
  name: 'Main',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.leftimg {
  float: left;
  width: 200px;
  margin-right: 3%;
}

.container {
  display: flex;
}

#item {
  text-align: right;
}
</style>
