QUESTIONNAIRES
======

A questionnaire is **a research instrument** consisting of a series of questions, for the purpose of gathering information from respondents.

Questionnaires are the product of **psychometric models**. Each psychometric model has its own questionnaires.

There are psychometric models to measure all sorts of things. We are interested in:
- Personality
- Intelelectual quotient (IQ)
- Career

## Personality

### Personality models

To measure personality, psychologists use **taxonomy models**.

The two main personality taxonomy models are the **Big Five (B5)** and the **HEXACO** model.

The structure of personality taxonomy models goes like this:

```
Domain 1
    Facet a
    Facet b
Domain 2
    Facet c
    Facet d
Domain 3
    Facet e
    Facet f
...
```

They asume **hierarchy**: facets belong to domains. 

They asume **lexicallity**: personality traits can be defined with words in human languages.

The difference between one taxonomy model and another is **how many domains and facets** there are, and in many cases **how they are lexically defined**.

Personality taxonomy models are valid to the extent that they are able to predict things such as academic performance, job performance, counterproductive work behaviour, wellbeing and mortality, and so on.

#### Big Five

The Big Five emerged in the early 1990s as a unifying taxonomy of personality traits. Collectively accounted for the major dimensions upon which individuals differ: Extraversion, Agreeableness, Conscientiousness, Neuroticism, and Intellect/openness.

#### HEXACO-PI

HEXACO is an acronym for six domains: Honesty-Humility (H), Emotionality (E), Extraversion (X), Agreeableness (A), Conscientiousness (C), and Openness to Experience (O).

In total, the HEXACO consists of 24 facets, four for each domain.

In 2007, HEXACO was updated. The second version is called HEXACO-REVISED. Two changes differentiate the HEXACO-PI-R from the previous HEXACO-PI: *Expressiveness* and *Negative Self-Evaluation* facets have been deleted, and *Social Self-Esteem* has been added.

#### Which is better?

Both frameworks offer a strong basis for examining individual differences in other traits.

If morally relevant behaviours are interesting, HEXACO model will often yield novel insights and improved prediction because of the honesty‐humility domain.

HEXACO is free for academic research. Anyone can [download Materials for Researchers](http://hexaco.org/hexaco-inventory) from their website. Big Five requires the payment of a fee.

### Personality questionnaires

Questionnaires have two elements:
- Questions
- Scoring key

Scoring key determines how to calculate facets from the answers to each question.

See [HEXACO Scoring Key](http://hexaco.org/downloads/ScoringKeys_100.pdf).

Questions must be translated to different languages by academic institutions and peer reviewed to be considered valid.

#### HEXACO Questionnaires

HEXACO has three different questionnaires, with different lenght:

- HEXACO Personality Inventory–Revised-60 (HEXACO-PI-R-60)
- HEXACO Personality Inventory–Revised-100 (HEXACO-PI-R-100)
- HEXACO Personality Inventory–Revised-200 (HEXACO-PI-R-200)

There are 24 facets, and an extra facet called *Altruism*. Thus, 25 facets.

The 100 questions questionnaire has 4 questions per each facet.
The 200 questions questionnaire has 8 questions per each facet.

#### How many questions are required?

Short‐form measures of personality should be avoided (i.e., measures with one to four items per scale). If researchers want to use a good relatively short measure, there are a range of good measures with between 8 and 12 items per factor.

Therefore, using the **HEXACO-PI-R-200 would be better** for scientific validation.

#### IPIP (International Personality Item Pool)

IPIP is an academic repository of personality questions. It's the psychollogy-equivalent of open software.

There are [3,320 IPIP Items](https://ipip.ori.org/AlphabeticalItemList.htm) in the IPIP database, free for anyone to copy, edit, translate, or use them for any purpose without asking permission and without paying a fee.

It's usually employed used when researchers wish to conduct their research on the Internet, and copyright restricts the copying and reformatting of items from commercial inventories.

If we ever create our own personality inventory, we would build it using IPIP.

## DEV

Check the [example folder](https://github.com/saiki-gg/questionnaires/tree/master/example) as a reference.

**RULES:**

- A folder per questionnaire with the three required .json files
- "name" attribute -> lowercase, no spaces (use - instead) and in english
- Numbers allways as number, never as a string

**TODO:**
- Data loader to the DB
- Update data if the json are updated

**IDEAS:**
- Just launch a command that checks if the folder and the jsons are valid
- If the jsons aren't correct get some clear feedback about the error and in which line
- `node loader.js hexaco-100` will create/update the `hexaco-100` folder
- `node loader.js hexaco-100 production` will launch the script agains the production DB

