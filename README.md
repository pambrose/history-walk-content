# History Walk Content

Slide content is defined using [Markdown](https://www.markdownguide.org/basic-syntax/)

## Required Elements

* Requires a variable named `slides`
* One slide must be marked as success with second slide variable
* Success and failure slides cannot have choices because they're the final slides

## Slide Example

```kotlin
slide("Slide Example") {
    content =
        """
            # Welcome to this slide example
            
            Here are some bullet points:
            * Item 1 with *italics*
            * Item 2 with **bold**   
        """

    verticalChoices() // or horizontalChoices()

    choice("Choice 1", "Choice 1 slide")
    choice("Choice 2", "Choice 2 slide")
    choice("Choice 3", "Choice 3 slide")
}
```

## Choice Alignment

Choices can be horizontally aligned with `horizontalChoices()`
or vertically aligned with `verticalChoices()`

