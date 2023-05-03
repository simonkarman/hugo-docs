---
title: "Images"
weight: 3
---

## Images
Add your image to `docs/static/images` directory and then use the following Markdown snippet to add them to your content.
```text
{\{< figure src="/images/<your-image-name>?width=60pc" >}}
# Note: Remove the initial \ in the above code, as it is their to avoid being drawn as an image. 
```

### Example
This is an example image, which is served as a static file (`boat.jpg`) from the `docs/static/images/` directory and displayed at a width of 40 percent (`?width=40pc`).

{{< figure src="/images/boat.jpg?width=40pc" >}}
