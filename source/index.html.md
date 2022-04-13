---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - python
  - shell

toc_footers:
  - <a href='https://dev3.daisi.io/my-tokens/api'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/slatedocs/slate'>Documentation Powered by Slate</a>

search: true

code_clipboard: true

meta:
  - name: description
    content: Documentation for the Kittn API
---

# Authentication
> To authorize, use this code:

```python
import os
os.environ["ACCESS_TOKEN"] = "'your token'"
```

```shell
-H "Authorization: token 'your token'"
```

> Make sure to replace `'your token'` with your personal access token.

You can access Daisi with or without personal access token 

You can register a new developer API key at our [developer portal](https://dev3.daisi.io/my-tokens/api).


<aside class="notice">
You must replace <code>'your token'</code> with your personal access token.
</aside>

# How to Use

## Install

```python
pip install pyDaisi
```

```shell

```

## Use
```python
from pydaisi import Daisi
daisi = Daisi("ImageColorization")
daisi.run(image="example_value")
```

```shell
curl -X POST "https://dev3.daisi.io/pebble-api/pebbles/1a1a932b-0ea2-4a3c-afe5-a6f723c8ce67/compute/run" -H "Content-Type: application/json" -d '{"image":"example_value"}' 
```

You could select the endpoints that defined in your daisi

### endpoint parameters

Parameter | Description
--------- | -----------
wait_for_completion | whether to send a asynchorous call to daisi backend, default is set to True

# Embed it into a document
`
<iframe title="ImageColorization Daisi" src="https://dev3.daisi.io/daisies/1a1a932b-0ea2-4a3c-afe5-a6f723c8ce67/embed" width="560" height="530" frameborder="0" />
`
