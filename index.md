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


<div class="row1">
    <center>
    <div style="float:left;margin-right:20px;">
        <img src="grossman.png" height="200" width="200" alt="aiden" />
        <p style="text-align:center;"><a href="https://aidengrossman.com">Aiden Grossman</a></p>
    </div>
    <div style="float:left;margin-right:20px;">
        <img class="middle-img" src="paehler.jpg" height="200" width="200" alt="ludger" />
        <p style="text-align:center;"><a href="https://ludger.fyi">Ludger Paehler</a></p>
    </div>
    <div style="float:left;margin-right:20px;">
        <img src="parasyris.jpg" height="200" width="200" alt="stinos" />
        <p style="text-align:center;"><a href="https://www.linkedin.com/in/kostadinos-parasyris-3992b950">Konstadinos Parasyris</a></p>
    </div>
    </center>
</div>

<div class="row2">
    <center>
    <div style="float:left;margin-right:20px;">
        <img src="ben-nun.jpg" height="200" width="200" alt="tal" />
        <p style="text-align:center;"><a href="https://tbennun.github.io">Tal Ben-Nun</a></p>
    </div>
    <div style="float:left;margin-right:20px;">
        <img class="middle-img" src="hegna.png" height="200" width="200" alt="jacob" />
        <p style="text-align:center;"><a href="https://www.linkedin.com/in/jacob-hegna">Jacob Hegna</a></p>
    </div>
    <div style="float:left;margin-right:20px;">
        <img src="moses.jpg" height="200" width="200" alt="william" />
        <p style="text-align:center;"><a href="https://wsmoses.com/academic/">William S. Moses</a></p>
    </div>
    </center>
</div>

<div class="row3">
    <center>
    <div style="float:left;margin-right:20px;">
        <img src="monsalve-diaz.jpg" height="200" width="200" alt="jose" />
        <p style="text-align:center;"><a href="https://www.anl.gov/profile/jose-manuel-monsalve">Jose Monsalve-Diaz</a></p>
    </div>
    <div style="float:left;margin-right:20px;">
        <img class="middle-img" src="trofin.png" height="200" width="200" alt="mircea" />
        <p style="text-align:center;"><a href="https://research.google/people/mircea-trofin/">Mircea Trofin</a></p>
    </div>
    <div style="float:left;margin-right:20px;">
        <img src="doerfert.jpg" height="200" width="200" alt="johannes" />
        <p style="text-align:center;"><a href="https://people.llnl.gov/doerfert1">Johannes Doerfert</a></p>
    </div>
    </center>
</div>

<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>

## Corresponding Author

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
