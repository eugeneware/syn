# syn & dic

Two simple shell scripts to use [wordnet]() to search for synonyms. Useful for finding names for your new modules.

Inspired by [substack](https://github.com/substack)'s approach to building modules (see this [blog post](http://substack.net/how_I_write_modules), and the comments in [this gist](https://gist.github.com/substack/5075355)).

In particular, these comments:


> Here are some naming tricks:
>
> * grep through /usr/share/dict/words with fragments of relevant words
> * apt-get install wordnet, then you can do wordnet $TERM -syns{n,v,a,r} to get lists of synonyms

## Installation

You need to have wordnet installed.

On Mac OSX:

```
$ brew install wordnet
```

On Linux:

```
$ apt-get install wordnet
```

Copy syn and dic into your $PATH, and then run it with a word to find a synonym for:

```
$ syn transform

Synonyms/Hypernyms (Ordered by Estimated Frequency) of verb transform

7 senses of transform

Sense 1
transform
       => change, alter, modify

Sense 2
transform, transmute, transubstantiate
       => change, alter, modify

Sense 3
transform, transmute, metamorphose
       => change

Sense 4
translate, transform
       => change, alter, modify

Sense 5
transform
       => change, alter, modify

Sense 6
transform
       => change, alter, modify

Sense 7
transform
       => change, alter, modify
```

And run ```dic``` to match words in ```/usr/share/dict/words```

```
$ dic transform
 autotransformer
 intertransformability
 intertransformable
 intransformable
 retransform
 retransformation
 transform
 transformability
 transformable
 transformance
 transformation
 transformationist
 transformative
 transformator
 transformer
 transforming
 transformingly
 transformism
 transformist
 transformistic
 untransformable
 untransformed
 untransforming
```

Enjoy!
