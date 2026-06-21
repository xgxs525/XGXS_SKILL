---
name: chinese-copy-review
description: Use this skill to review, humanize, and optimize Chinese self-media copy, including Douyin oral scripts, WeChat Official Account posts, Weibo posts, Xiaohongshu notes, Moments posts, and Video Channel scripts. It preserves the user's original meaning while checking logic, grammar, sensitive wording, short-sentence density, repetition, punctuation, examples, transitions, oral delivery, and AI-like phrasing, then outputs a complete revised version.
---

# 中文文案全流程检查与优化 Skill

## Use this skill when

Use this skill whenever the user asks to modify, polish, check, simplify, humanize, de-AI, oralize, or optimize Chinese self-media copy, especially for:

- 抖音口播
- 视频号口播
- 小红书文案
- 微博文案
- 公众号文章
- 朋友圈文案
- 自媒体短视频脚本
- 成长类、情绪类、人生感悟类、个人表达类文案

Typical user requests include:

- “检查全文案”
- “去 AI 味”
- “改得更像真人说话”
- “口播自然一点”
- “检查语病逻辑”
- “检查敏感词”
- “短句合并”
- “去掉重复”
- “标点符号调整”
- “上下文顺一下”
- “按 Skill 改”
- “最后把修改后的完整文案列出来”

## Primary goal

Preserve the user's original meaning, tone, emotion, narrative order, and core point while making the copy:

- more natural
- more human
- easier to understand
- smoother for oral delivery
- less repetitive
- less AI-like
- safer for public posting
- ready to use as a complete final draft

Do not rewrite the copy into a completely different article unless the user explicitly asks for a heavy rewrite.

## Core principles

### 1. Preserve original intent

Keep the user's original topic, viewpoint, mood, examples, narrative angle, and character setting as much as possible.

Allowed changes:

- word order
- punctuation
- sentence merging
- oral expression
- repeated wording
- unnatural sentence patterns
- transitions
- grammar and logic issues
- risky or sensitive wording

Avoid adding without user request:

- new viewpoints
- new stories
- new examples
- new positions
- forced quotes
- forced inspirational endings
- excessive emotional elevation
- obvious AI-style summaries

### 2. Remove obvious AI tone

Always check for AI-like writing.

Avoid making the copy too:

- neat
- complete
- correct-sounding
- symmetrical
- slogan-like
- abstract
- over-explained
- over-polished

Be especially careful with repeated use of these patterns:

- “不是……而是……”
- “与其……不如……”
- “我们都要……”
- “真正的……”
- “很多人都以为……”
- “其实……”
- “你要明白……”
- “到最后你会发现……”

These patterns are not banned, but they must not appear too densely.

### 3. Optimize for oral delivery

For Douyin, Video Channel, Xiaohongshu, or other spoken scripts, prioritize whether the text sounds natural when read aloud.

Check whether:

- the rhythm is smooth
- the pauses are natural
- the wording sounds like real speech
- the sentences are too fragmented
- the writing feels too much like an article
- the explanation is too long
- the user can read it directly without awkwardness

Short sentences can be kept when they create rhythm or emphasis. Do not merge all short sentences automatically.

### 4. Do not over-edit

If the user's original sentence is already clear, natural, and useful, keep it.

Do not make simple language more complex just to sound “advanced”.

Do not add literary phrasing unless it genuinely improves the user's intended style.

## Default workflow

When the user asks for a general review or says “按 Skill 改”, perform the following checks in order:

1. Logic and grammar
2. Simplicity and clarity
3. Sensitive or risky wording
4. Excessive short sentences
5. Repetition in adjacent sentences
6. Punctuation
7. Natural oral expression
8. Repeated or unnecessary examples
9. Abrupt transitions
10. Full-text final review
11. Add natural quotable lines only if requested
12. Replace celebrity names only if requested
13. Output the complete revised copy

## Task modules

### Module 1: Logic and grammar check

Trigger when the user says:

- “语病逻辑”
- “检查逻辑问题”
- “检查语病”
- “这段话通不通”
- “有没有表达问题”

Check for:

- awkward sentences
- unclear subject or object
- mismatched sentence parts
- contradictory logic
- weak cause-and-effect
- unnatural transitions
- repeated explanations
- wording that normal people would not say

Preferred output:

```markdown
### 语病和逻辑问题

原句：
修改：
问题：

### 修改后的完整文案

正文
```

### Module 2: Simplicity and sensitive wording

Trigger when the user says:

- “简单敏感词”
- “检查敏感词”
- “改得简单点”
- “检查有没有违规词”
- “帮我规避敏感表达”

First, identify places that can be simpler and easier to understand.

Then check and soften high-risk wording related to:

-刑罚、牢狱、违法犯罪
-毒品
-赌博
-暴力、恐怖、伤害
-色情、低俗、擦边
-迷信、算命、招财、改运
-地域歧视、种族歧视、民族宗教歧视
-党政领导、英烈历史、国家安全
-非法金融、虚拟币炒作、保本高息
-虚假宣传和极限夸大
-侮辱性、攻击性、脏话
-非法办证、假币、黑产

When sensitive wording appears, replace it with neutral, moderate, platform-friendly wording.

Examples:

- “稳赢” → “更稳妥”
- “百分百有效” → “可能会更有帮助”
- “全网第一” → “比较有代表性”
- “傻” → “不太清楚”
- “毁掉” → “影响”
- “爆发” → “出现明显变化”

Important: This is public-posting risk optimization, not a legal review. Do not over-delete normal expressions.

### Module 3: Short-sentence merging

Trigger when the user says:

- “短句合并”
- “检查短句”
- “把太短的句子合并”
- “让口播更顺”
- “不要一句一句太碎”

Check whether the copy has too many short sentences that could naturally be connected with commas.

Merge when:

- several short sentences express one continuous idea
- the text sounds mechanical
- the pauses are too frequent
- it feels like AI-style line breaks

Keep short sentences when:

- they create emphasis
- they carry emotion
- they mark a turn
- they are important rhythm points

Do not turn everything into long sentences.

### Module 4: Repetition cleanup

Trigger when the user says:

- “去掉重复”
- “检查重复词”
- “检查相邻句子重复”
- “重复开头太多”
- “同一个词出现太多”

Handle two types of repetition.

#### Adjacent sentence repetition

Check for repeated:

- openings
- keywords
- sentence patterns
- expression structures

If repetition is dense, merge, delete, or rephrase. Do not remove all repetition, because some repetition creates oral rhythm.

#### Same word appearing 3 or more times in nearby sentences

If the same word appears 3 or more times in adjacent sentences, adjust it.

If it appears only twice, it can usually stay.

Preferred output:

```markdown
### 重复问题修改

原句：
修改：
问题：

### 修改后的完整文案

正文
```

### Module 5: Punctuation cleanup

Trigger when the user says:

- “标点符号”
- “检查标点”
- “标点改一下”
- “去掉多余标点”
- “不要破折号”

Rules:

- Do not change punctuation just because it “looks uncomfortable”.
- Use semicolons rarely.
- Remove unnecessary colons when they make the line stiff.
- Use commas to connect continuous short thoughts.
- Do not use em dashes or Chinese破折号.
- Avoid excessive exclamation marks.
- Avoid excessive ellipses.
- Preserve natural pauses for oral delivery.
- Break overly long sentences with periods.

### Module 6: Natural expression check

Trigger when the user says:

- “正常表达”
- “像正常人说话”
- “口播自然点”
- “不要太书面”
- “去掉不自然表达”
- “像真人说话”

Check whether the copy sounds like something a real person would say.

Fix:

- overly formal language
- overly complete explanations
- stiff phrasing
- abstract wording
- too many big concepts
- sentences that go too far around the point
- awkward oral rhythm
- obvious AI-generated phrasing

Preferred output:

```markdown
### 表达修改

原句：
修改：
问题：

### 修改后的完整文案

正文
```

### Module 7: Example de-duplication

Trigger when the user says:

- “例子去重”
- “检查例子”
- “例子是不是太多”
- “哪些例子可以删”
- “把多余例子删掉”

List every example in the copy, then decide whether each should be:

- kept
- deleted
- replaced
- merged

Decision rules:

- Keep examples that are vivid, relevant, and not repetitive.
- Delete examples that repeat the same point or add no new information.
- Replace examples that feel unnatural, distant, or unsuitable for oral delivery.
- Merge examples that express the same idea.

Preferred output:

```markdown
### 例子检查

例子 1：
处理方式：保留 / 删除 / 替换 / 合并
原因：

### 修改后的完整文案

正文
```

### Module 8: Transition and flow check

Trigger when the user says:

- “衔接突兀”
- “上下文不顺”
- “过渡不自然”
- “前后接不上”
- “帮我顺一下前后逻辑”

Check for:

- sudden topic jumps
- unclear relation between sentences
- emotional turns that are too abrupt
- missing bridge between example and point
- endings that arrive too suddenly
- weak opening setup
- disconnected middle sections

Fix by:

- adding light transitions
- adjusting sentence order
- merging related ideas
- deleting abrupt lines
- softening hard transition words
- letting the tone move naturally

Preferred output:

```markdown
### 衔接问题

原文位置：
问题：
修改建议：

### 修改后的完整文案

正文
```

### Module 9: Full-text review

Trigger when the user says:

- “全文检查”
- “再整体看一遍”
- “看看还有什么问题”
- “还有哪些地方可以改”
- “最后完整优化一下”

Check everything together:

- logic
- grammar
- repetition
- wordiness
- AI tone
- oral delivery
- short-sentence density
- punctuation
- sensitive wording
- examples
- transitions
- simplicity

Preferred output:

```markdown
### 全文问题

问题 1：
修改方式：

问题 2：
修改方式：

### 修改后的完整文案

正文
```

### Module 10: Add natural quotable lines

Only use this module when the user explicitly asks to add quotable lines or “金句”.

Do not add quotable lines by default.

Good quotable lines should be:

- natural
- short
- easy to remember
- not too polished
- not like generic motivational copy

Avoid:

- forced inspiration
- forced rhyme
- excessive elevation
- empty correctness
- template-like public-account style
- success-mindset slogans

Preferred output:

```markdown
### 金句插入位置

金句 1：
插入位置：

金句 2：
插入位置：

金句 3：
插入位置：

金句 4：
插入位置：

### 修改后的完整文案

正文
```

### Module 11: Replace celebrity or famous-person names

Only use this module when the user explicitly asks to remove or generalize names.

Replace specific names with general phrases such as:

- 一个很厉害的人
- 一个很有成就的人
- 一个做得很好的人
- 一个很有代表性的人
- 那些真正把事做成的人
- 一个在这个领域走得很远的人

Do not change the function of the example.

If the user asks whether this is better, explain briefly: generalizing names can make oral copy less distracting and reduce unnecessary debate, but if the name is the core example, do not erase it completely.

### Module 12: Complete final draft output

Trigger when the user says:

- “全文列出来”
- “最后把完整文案列出来”
- “按你的建议调整一版”
- “直接给我最终版”

Always output a complete revised version.

Do not only provide suggestions.

Do not say “已调整” without giving the full text.

Do not make the user assemble changes manually.

## Output rules

Choose the output structure based on the user's request.

### If the user asks to list problems

```markdown
### 检查结果

原句：
修改：
问题：

原句：
修改：
问题：

### 修改后的完整文案

正文
```

### If the user only asks for one revised version

```markdown
### 修改后的完整文案

正文
```

### If the user asks for suggestions first

```markdown
### 修改建议

1.
2.
3.

### 修改后的完整文案

正文
```

### If the user asks to list every change

```markdown
### 改动说明

原句：
修改：
原因：

原句：
修改：
原因：

### 修改后的完整文案

正文
```

## Editing intensity

### Light edit

Use when the user says:

- “轻微改一下”
- “基本不动”
- “保留原文”
- “只检查问题”

Only fix clear problems.

### Medium edit

Use when the user says:

- “调整一版”
- “顺一下”
- “改自然点”
- “去 AI 味”

Keep the original structure and improve expression, transitions, repetition, and oral rhythm.

### Heavy edit

Use when the user says:

- “重新整理”
- “重写一版”
- “大改”
- “按你的判断改”

You may adjust structure and paragraph order, but still preserve the user's core meaning.

## Default behavior

When the user provides copy and says “按这个 Skill 改”, default to:

- check logic and grammar
- simplify wordy expression
- soften sensitive wording
- merge excessive short sentences
- reduce dense repetition
- adjust punctuation
- improve oral naturalness
- smooth transitions
- reduce obvious AI tone
- output the complete revised copy

Do not default to:

- adding quotable lines
- removing names
- heavily rewriting structure
- expanding content
- changing the topic
- changing the persona
- changing the story background

Only do those when the user explicitly asks.

## Final response requirement

Every completed review must include:

```markdown
### 修改后的完整文案
```

Then provide the full revised copy.

Never leave the user with only suggestions.

Never make the user piece together the final draft.

## Quick user command

The user can invoke this skill by saying:

```text
按中文文案全流程 Skill 检查这篇文案，保留原意，去掉 AI 味，让口播更自然，最后把修改后的完整文案列出来。
```

When this command appears, apply this skill directly.
