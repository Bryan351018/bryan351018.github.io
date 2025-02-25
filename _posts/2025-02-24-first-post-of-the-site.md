---
title:  "First post on this website!"
needs_math: true
needs_chem: true

toc: true
toc_label: "Quick jump"
toc_icon: "file-alt"

license: "CC 0"
---

# Hello there!

This is the first post ever created on [bryan351018.github.io](https://bryan351018.github.io/).
But you might ask: what is this website?

## Backbones
The website that you're seeing right now is built on top of two **monstrous** third-party projects: [Jekyll](https://jekyllrb.com/) and [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/).

### Jekyll
Websites are ultimately displayed from HTML, CSS, and JavaScript. While it is *possible* to make an entire website from these (such as my [JavaScript Projects](/projects/javascript/), though they are more appropriately called "web apps"), it can get incredibly **tedious** and **repetitive**.

This is where Jekyll comes in. Instead of having to worry about the repetitive aspects like menubars and formatting, Jekyll allows you to configure once, and not have to worry about it for a long time. This allows you to focus mainly on the high-level contents of the websites, instead of the technical details.

Jekyll combines [Markdown](https://www.markdownguide.org/), HTML, and [YAML](https://yaml.org/) into an entire website. **Markdown** is used for the post, article, and menubar contents, while **YAML** is used for configuration files for the website.

This post was written in Markdown, for example. Feel free to peek at the [source document](https://github.com/Bryan351018/bryan351018.github.io/blob/master/_posts/2025-02-03-first-post-of-the-site.md?plain=1).


### Minimal Mistakes
Minimal Mistakes is a Jekyll plugin that provides many convenient features, including automatic styling, page and article templates, automatic search and comments integration, optional layouts, custom themes, and a lot more.

### Why not use a commercial content management system?
While services like Wix.com, Shopify, Squarespace, and WordPress do exist, and they have a more intuitive interface for people not experienced with programming... They are **not** a great fit once the website grows larger and larger, since the visual manipulation of the webpage elements can be time-consuming and *pretty inefficient*.

Plus, Jekyll and Minimal Mistakes are **open-source** projects with hundreds to thousands of contributors, making and discussing changes almost every month. This means they tend to be more actively maintained and less buggy compared to commercial alternatives.

## Features

### Markdown
Markdown is a simple and intuitive markup language, with features like
- Bulleted lists
  - Multi-level lists

1. Numbered lists
> Block quotes

And even code:

```cpp
using namespace std;

int main() {
    try {
        std::vector<int> vec{3, 4, 3, 1};
        int i{vec.at(4)}; // Throws an exception, std::out_of_range (indexing for vec is from 0-3 not 1-4)
    } catch (const std::out_of_range& e) {
        // An exception handler, catches std::out_of_range, which is thrown by vec.at(4)
        std::println(stderr, "Accessing a non-existent element: {}", e.what());
    } catch (const std::exception& e) {
        // To catch any other standard library exceptions (they derive from std::exception)
        std::println(stderr, "Exception thrown: {}", e.what());
    } catch (...) {
        // Catch any unrecognised exceptions (i.e. those which don't derive from std::exception)
        std::println(stderr, "Some fatal error");
    }

    return 0;
}
```

```python
n = int(input('Type a number, and its factorial will be printed: '))

if n < 0:
    raise ValueError('You must enter a non-negative integer')

factorial = 1
for i in range(2, n + 1):
    factorial *= i

print(factorial)
```

```javascript
function print_hello()
{
    console.log("Hello World!")
    return true;
}
```

### Mathematics and chemistry rendering
By enabling a configuration for this post, it can display inline math equations such as \\( f(z) = z^3 - 1, \ z \in \mathbb{C} \\),
and even inline chemical entities like \\( \ce{H2O} \\). This is done thanks to the [\\( \KaTeX \\) library](https://katex.org/).

Centered math equations and chemical entities can also be displayed, and they look even *better*:
\\[ \sigma = \sqrt{ \frac{1}{N} \sum_{i=1}^N (x_i -\mu)^2} \\]

\\[ C_p[\ce{H2O(l)}] = \pu{75.3 J // mol K} \\]

Try **copying** any of the equations above, and pasting it somewhere else! It will paste as \\( \LaTeX \\) code (for browsers that support it).

# Go forth!
There's a comment section at the end of the page that you can play around with, but otherwise, thanks for showing interest in my website! See you soon.
