# ABAP Expert — Claude skill

Claude'u kıdemli bir SAP ABAP geliştirici / teknik danışman gibi çalıştıran skill:
clean core (Level A–D), modern ABAP (ECC → ABAP Cloud, RAP, CDS), kod yazma, code review,
ST22 dump analizi, debugging ve performans analizi.

Skill içeriği: [`skills/abap-expert/SKILL.md`](skills/abap-expert/SKILL.md)

## 1) Claude chat (claude.ai / Claude Desktop) — en basit yol

1. Zip'i indir: **[abap-expert.zip](https://github.com/furkanakdag/abap-expert-skill/raw/main/abap-expert.zip)**
2. Claude'da **Settings → Capabilities → Skills** bölümünü aç (gerekirse "Code execution and file creation" açık olmalı).
3. **Upload skill** ile zip'i yükle ve skill'i aktif et.
4. Yeni bir sohbette ABAP sorusu sor; Claude skill'i otomatik kullanır. İstersen
   "abap-expert skill'ini kullan" diyerek açıkça da çağırabilirsin.

> Not: Repodaki "Code → Download ZIP" dosyası değil, yukarıdaki `abap-expert.zip` yüklenmeli.

## 2) Claude Code — tek komutla

Claude Code içinde:

```
/plugin marketplace add furkanakdag/abap-expert-skill
/plugin install abap-expert@abap-expert-skill
```

Alternatif (manuel):

```bash
git clone https://github.com/furkanakdag/abap-expert-skill
mkdir -p ~/.claude/skills
cp -r abap-expert-skill/skills/abap-expert ~/.claude/skills/
```

## Güncelleme

Claude chat: yeni `abap-expert.zip`'i indirip skill'i yeniden yükle.
Claude Code: `/plugin marketplace update abap-expert-skill`.
