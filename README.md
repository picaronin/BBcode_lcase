[![phpBB](https://www.phpbb-es.com/foro/styles/flat-style/theme/images/logo_new_small.png)](https://www.phpbb-es.com/foro/viewtopic.php?f=84&t=43039)
# BBcode lcase
With this BBcode for phpBB the actual transformation of the selected text is achieved since Uppercase to Lowercase.

### BBCode usage:
```
[lcase]{TEXT}[/lcase]
```

### HTML replacement:
```
<span id="lcase1000">{TEXT}</span>
<script>
    var res = document.getElementById("lcase1000").innerHTML.toString().toLowerCase();
    var uniqid = Math.random().toString(36).replace(/[^a-z]+/g, '').substr(2, 10);
    document.getElementById("lcase1000").setAttribute("id", uniqid);
    document.getElementById(uniqid).innerHTML = res;
</script>
```

### Help line:
```
[lcase]TEXT[/lcase] Uppercase to Lowercase
```
