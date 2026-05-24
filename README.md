# note-writer-zh

`note-writer-zh` is a Codex skill for generating and organizing Chinese study notes.
It is designed for lecture notes, textbook notes, review materials, and reading notes that need to be natural, formal, rigorous, and less template-like.

The skill emphasizes:

- chapter-by-chapter development instead of fixed review templates;
- precise definitions, theorems, algorithms, formulas, proofs, and examples;
- independent blocks for important concepts and results;
- Chinese prose that is fluent and written, while keeping mathematical and technical conditions explicit;
- a Typora-friendly `note.css` theme for clean note blocks.

## Acknowledgement

The writing cleanup rules in this skill were informed by `humanizer-zh`, especially its guidance on reducing formulaic openings, promotional wording, vague attribution, forced three-part structures, and other common machine-written patterns. The relevant guidance has been rewritten into this skill so `note-writer-zh` can be used independently without requiring `humanizer-zh` to be installed.

## Files

- `SKILL.md`: the skill instructions.
- `agents/openai.yaml`: Codex skill metadata.
- `assets/note.css`: Typora/Markdown CSS for note blocks and a warm paper-like page style.

## Typora Usage

Copy or install `assets/note.css` into Typora's theme directory, then select the theme named `note`.

Recommended Markdown block syntax:

```markdown
> <span class="note-title note-definition-title">定义 1.1（概念名）</span>
>
> 这里写严格定义。定义中的对象、条件和边界要完整。
```

```markdown
> <span class="note-title note-algorithm-title">算法 1.1（算法名）</span>
>
> - 适用条件：...
> - 基本思路：...
> - 时间复杂度：...
```
