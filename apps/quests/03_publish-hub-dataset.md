# Week 2: Publish a Hub Dataset

Create and share high-quality datasets on the Hub. Good data is the foundation of good models—help the community by contributing datasets others can train on.

## Why This Matters

The best open source models are built on openly available datasets. By publishing well-documented, properly structured datasets, you're directly enabling the next generation of model development. Quality matters more than quantity.

## The Skill

Use `skills/huggingface-datasets/` for this quest. Key capabilities:

- Initialize dataset repos with proper structure
- Multi-format support: chat, classification, QA, completion, tabular
- Template-based validation for data quality
- Streaming uploads without downloading entire datasets

```bash
# Create the dataset repo (or reuse an existing one)
hf repos create your-username/dataset-name --type dataset --exist-ok
```

## XP Tiers

### 🐢 Starter — 50 XP

**Upload a small, clean dataset with a complete dataset card.**

1. Create a dataset with ≤1,000 rows
2. Write a dataset card covering: license, splits, and data provenance
3. Upload to the Hub under the hackathon organization (or your own account)

**What counts:** Clean data, clear documentation, proper licensing.

```bash
hf repos create hf-skills/your-dataset-name --type dataset --exist-ok

hf upload hf-skills/your-dataset-name ./your_data.json data --type dataset
```

### 🐕 Standard — 100 XP

**Publish a conversational dataset with a complete dataset card.**

1. Create a dataset with ≤1,000 rows
2. Write a dataset card covering: license and splits.
3. Upload to the Hub under the hackathon organization.

**What counts:** Clean data, clear documentation, proper licensing.

### 🦁 Advanced — 200 XP

**Translate a dataset into multiple languages and publish it on the Hub.**

1. Find a dataset on the Hub
2. Translate the dataset into multiple languages
3. Publish the translated datasets on the Hub under the hackathon organization

**What counts:** Translated datasets and merged PRs.

## Resources

- [SKILL.md](../../skills/huggingface-datasets/SKILL.md) — Full skill documentation

---

**Next Quest:** [Supervised Fine-Tuning](04_sft-finetune-hub.md)
