<script src="[https://cdn.jsdelivr.net/npm/marked/marked.min.js](https://rawcdn.githack.com/CandelaSolutions/.github/08f1985bbe6be0aea24ed897829d0095f04feb72/profile/scripts/marked.min.js)"></script>
<script>
    fetch('https://rawcdn.githack.com/CandelaSolutions/filament/f3e9603c8f5701bc183b2d2c0145a72a925c8d8d/README.md')
        .then(response => response.text())
        .then(markdown => {
            const htmlContent = marked(markdown);
            document.getElementById('remote-markdown-content').innerHTML = htmlContent;
        })
        .catch(error => console.error('Error fetching markdown:', error));
</script>

# Filament

<div id="remote-markdown-content"></div>
