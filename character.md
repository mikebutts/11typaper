---
layout: layout.liquid
title: Rice & Morty Characters
pagination:
  data: characters
  alias: character
  size: 1
permalink: "/character/{{ character.name|slug}}/"
---

## {{character.name}}

{{ character | dump}}

{{character.name}}
{{character.image}}
<a href="/characters"> Go back to characters </a>
