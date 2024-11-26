---
title: 'Wyzardry-Engine'
description: 'Here is a sample of some basic Markdown syntax that can be used when writing Markdown content in Astro.'
pubDate: '11/19/2024'
# heroImage: '/blog-placeholder-1.jpg'
---

Here is a sample of some basic Markdown syntax that can be used when writing Markdown content in Astro.

## Headings

The following HTML `<h1>`—`<h6>` elements represent six levels of section headings. `<h1>` is the highest section level while `<h6>` is the lowest.

# H1

## H2

### H3

#### H4

##### H5

###### H6

## Paragraph -->

  The Wizardry Engine is a physic engine made as a project for the first module at SAE Institute, it riquiers physics and demonstrations of said physics.


<!-- ## Images

### Syntax

```markdown
![Alt text](./full/or/relative/path/of/image)
```

### Output

![blog placeholder](/blog-placeholder-about.jpg) -->

### Blockquote without attribution

#### Syntax

```markdown
> void GraphicManager::CreateCircle(core::Vec2<float> pos, float radius, SDL_Color color)
{
	// Get the size of the idx_vector as the starting idx
	const std::size_t starting_idx = vertices_.size();

	float angle_step = 2.0f * 3.14f / static_cast<float>(num_segments);

	AddVertex(pos, color);

	// Draw triangles for the radius of the circle
	for (std::size_t i = 0; i < num_segments; i++)
	{
		float angle = i * angle_step;
		float x = pos.x + radius * std::cos(angle);
		float y = pos.y + radius * std::sin(angle);

		AddVertex(core::Vec2<float>(x, y), color);
	}

	// Give an id to every segments
	for (int i = 0; i < num_segments - 1; i++)
	{
		idx_vertices_.push_back(starting_idx);
		idx_vertices_.push_back(starting_idx + i + 1);
		idx_vertices_.push_back(starting_idx + i + 2);
	}

	// Put back the first segment as the last one after going through the whole vector
	idx_vertices_.push_back(starting_idx);
	idx_vertices_.push_back(starting_idx + num_segments);
	idx_vertices_.push_back(starting_idx + 1);
}
```

#### Output

> Here's, for start, the draw circle fonction.  
> Only works on the graphyc side of things

### Blockquote with attribution

#### Syntax

```markdown
> Don't communicate by sharing memory, share memory by communicating.<br>
> — <cite>Rob Pike[^1]</cite>
```

#### Output

> Don't communicate by sharing memory, share memory by communicating.<br>
> — <cite>Rob Pike[^1]</cite>

[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

## Tables

### Syntax

```markdown
| Italics   | Bold     | Code   |
| --------- | -------- | ------ |
| _italics_ | **bold** | `code` |
```

### Output

| Italics   | Bold     | Code   |
| --------- | -------- | ------ |
| _italics_ | **bold** | `code` |

## Code Blocks

### Syntax

we can use 3 backticks ``` in new line and write snippet and close with 3 backticks on new line and to highlight language specific syntax, write one word of language name after first 3 backticks, for eg. html, javascript, css, markdown, typescript, txt, bash

````markdown
```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>Example HTML5 Document</title>
  </head>
  <body>
    <p>Test</p>
  </body>
</html>
```
````

### Output

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>Example HTML5 Document</title>
  </head>
  <body>
    <p>Test</p>
  </body>
</html>
```

## List Types

### Ordered List

#### Syntax

```markdown
1. First item
2. Second item
3. Third item
```

#### Output

1. First item
2. Second item
3. Third item

### Unordered List

#### Syntax

```markdown
- List item
- Another item
- And another item
```

#### Output

- List item
- Another item
- And another item

### Nested list

#### Syntax

```markdown
- Fruit
  - Apple
  - Orange
  - Banana
- Dairy
  - Milk
  - Cheese
```

#### Output

- Fruit
  - Apple
  - Orange
  - Banana
- Dairy
  - Milk
  - Cheese

## Other Elements — abbr, sub, sup, kbd, mark

### Syntax

```markdown
<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd>CTRL</kbd> + <kbd>ALT</kbd> + <kbd>Delete</kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.
```

### Output

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd>CTRL</kbd> + <kbd>ALT</kbd> + <kbd>Delete</kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.

<a href=[lien](https://github.com/Tornade-10/Wizardry-engine.git)>[Project Github]</a>


[Wizardry-engine.git](https://github.com/Tornade-10/Wizardry-engine.git)