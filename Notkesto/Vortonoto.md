---
date: 2023-08-05
type: 🧠
aliases:
  - Vortonotoj
---

**Topics:** [[Notkesto]] - [[Types of Notes]]

---

A _Vortonoto_ (Esperanto for "word note"; pl. _Vortonotoj_) is the type of note that is used to write down vocabulary (or sentences) that I learn in a specific language.

The purpose of these notes is not only to contain this vocabulary, but also to export it to [Anki](https://apps.ankiweb.net/) via the [Obsidian_to_Anki Obsidian plugin](https://github.com/Pseudonium/Obsidian_to_Anki). Anki is a [[Spaced-Repetition|spaced-repetition]] program that I use to memorise and practice new vocabulary.

As of August 2023, this export process only contemplates vocabulary and sentences. I additionally use the [QuickAdd Obsidian plugin](https://github.com/chhoumann/quickadd) to quickly capture the vocabulary or sentences that go into these notes.

In the future, I plan on writing a [blog](https://psycake.subspace.club/) entry about this whole workflow. I will update this note whenever it's published, but in the meantime, here's the basic rundown of how these notes are structured and processed.

# Vocabulary

Vocabulary is written in the following format:

| • \[word/construction] | \[definition/translation\]  |
| ---------------------- | --------------------------- |
| \[example sentence\]   | \[translation of sentence\] |
| \[part of speech\]     | \[extra information\]       |
<!--ID: 1699812638234-->

Obsidian_to_Anki captures each of these tables with the following RegEx:

```regex
\| • ([^\n|]+)\|([^\n|]+)\|\n\|[^\n|]+\|[^\n|]+\|\n\|([^\n|]+)\|([^\n|]+)\|\n\|([^\n|]+)\|([^\n|]+)\|\n?()()()
```

For vocabulary, I use a custom-made vocabulary-focused Anki note type with the following fields:

1. Word (front)
2. Definition (back)
3. Foreign sentence
4. Translated sentence
5. Part of speech
6. Extra
7. IPA
8. ID
9. Rank

Notice that the first 6 fields are filled with the contents of each table, while the last 3 are simply left empty (I either don't need them everytime or fill them within Anki). This is why the RegEx has `()()()` at the very end of it.

# Sentences

Sentences are written in the following format:

| - \[foreign sentence\] | \[translated sentence\] |
| ---------------------- | ----------------------- |
<!--ID: 1699812638232-->

Obsidian_to_Anki captures each of these tables with the following RegEx:

```regex
\| - ([^\n|]+)\|([^\n|]+)\|\n\|[^\n|]+\|[^\n|]+\|\n?()()
```

For sentences, I use a custom-made general-purpose Anki note type with the following fields:

1. Front
2. Back
3. Extra
4. ID

Notice it's basically a basic note type on steroids. The first two fields are filled with the contents of each table, while the last two are left empty (hence the `()()` at the end of the RegEx).

# Metadata

Vortonotoj are marked by the `🌐` [[Types of Notes|type]].

In addition, all Vortonotoj contain the following YAML metadata that Obsidian_to_Anki reads:

- `anki-deck`, which contains the target Anki deck where every generated note will go
- `anki-tags`, which contains the desired Anki tags for every generated note
