## ROT13 Converter
### About Webpage

HTML Webpage for ROT 13 Conversion with Javascript 
Made By @gk2savage @tanveer9xo
- Rot 13 or Rot <any number> Conversion on this Webpage

^ function rot(s, i) {
      return s.replace(/[a-zA-Z]/g, function (c) {
        return String.fromCharCode((c <= 'Z' ? 90 : 122) >= (c = c.charCodeAt(0) + i) ? c : c - 26);
      });
    }
    function update() {
      document.getElementById('output').value = rot(document.getElementById('input').value, +document.getElementById('rot').value);
    }
