make /wp-content/themes/twentyseventeen/template-parts/post/content.php

```
# 32 line
the_content( sprintf(
	__( 'Continue reading<span class="screen-reader-text"> "%s"</span>', 'twentyseventeen' ),
	get_the_title()
) );
```

change to

```
the_markdown_content( sprintf(
	__( 'Continue reading<span class="screen-reader-text"> "%s"</span>', 'twentyseventeen' ),
	get_the_title()
) );
```
