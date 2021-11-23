# History Walk Content

Slide content is defined using [Markdown](https://www.markdownguide.org/basic-syntax/)

## Required Elements

* Requires a variable named `slides`
* One slide must be marked as success (with second slide argument)
* Success and failure slides cannot have choices because they're terminal slides

## Slide Example

```kotlin
slide("Slide Example") {
  addText(
    """
            # Welcome to this slide example
            
            Here are some bullet points:
            * Item 1 with *italics*
            * Item 2 with **bold**   
        """
  )

  addImage("https://www.source.com/image.jpg", 300, 300)

  verticalChoices() // or horizontalChoices()

  addChoice("Choice 1", "Choice 1 slide")
  addChoice("Choice 2", "Choice 2 slide")
  addChoice("Choice 3", "Choice 3 slide")
}
```

## Choice Alignment

Choices can be horizontally aligned with `horizontalChoices()`
or vertically aligned with `verticalChoices()`

