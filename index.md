---
layout: default
title: ComPile
---


## Abstract

Code is increasingly becoming a core data modality of modern machine learning research impacting not only the way we write code
with conversational agents like OpenAI's ChatGPT, Google's Bard, or Anthropic's Claude, the way we translate code from one language
into another, but also the compiler infrastructure underlying the language. While modeling approaches may vary and representations differ,
the targeted tasks often remain the same within the individual classes of models. Relying solely on the ability of modern models to extract
information from unstructured code does not take advantage of 70 years of programming language and compiler development by not utilizing the
structure inherent to programs in the data collection. This detracts from the performance of models working over a tokenized representation
of input code and precludes the use of these models in the compiler itself. To work towards better intermediate
representation (IR) based models, we fully utilize the LLVM compiler infrastructure, shared by a number of languages, to generate
a 182B token dataset of LLVM IR. We generated this dataset from programming languages built on the shared LLVM
infrastructure, including Rust, Swift, Julia, and C/C++, by hooking into LLVM code generation either through the language's package
manager or the compiler directly to extract the dataset of intermediate representations from production grade programs.
Our dataset shows great promise for large language model training, and machine-learned compiler components.

## The Different Aspects of the Dataset Visualized

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)

## Authors

* Aiden Grossman
* Ludger Paehler
* Konstantinos Parasyris
* Tal Ben-Nun
* Jacob Hegna
* William S. Moses
* Jose M Monsalve Diaz
* Mircea Trofin
* Johannes Doerfert

## Corresponding Authors

* Aiden Grossman ([amgrossman@ucdavis.edu](mailto:amgrossman@ucdavis.edu?subject=ComPile))

## Citation

```bibtex
@article{grossman2023compile,
  title={ComPile: A Large IR Dataset from Production Sources},
  author={Grossman, Aiden and Paehler, Ludger and Parasyris, Konstantinos and Ben-Nun, Tal
          and Hegna, Jacob and Moses, William and Diaz, Jose M Monsalve and Trofin, Mircea
          and Doerfert, Johannes},
  journal={arXiv preprint arXiv:2309.15432},
  year={2023}
}
```
