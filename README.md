# AutoShorts

> Transforme lives de gaming em Shorts virais automaticamente.

AutoShorts é uma ferramenta desktop que analisa vídeos longos (lives, gameplays) e extrai automaticamente os melhores momentos, gerando clipes verticais prontos para TikTok, Reels e YouTube Shorts — com legenda sincronizada incluída.

---

## O que faz

- **Detecta momentos automaticamente** — análise de picos de áudio + IA (Gemini 2.5 Flash) identifica os trechos mais interessantes do vídeo
- **Revisão antes de cortar** — interface lista os momentos detectados com score e contexto; o usuário aprova quais quer processar
- **Crop vertical 9:16** — corte central para formato mobile, sem perder conteúdo importante
- **Legendas sincronizadas** — transcrição via Whisper com timing palavra-por-palavra; exporta `.srt` editável
- **Interface gráfica completa** — sem precisar de terminal; configuração visual por vídeo
- **Processamento em lote** — múltiplos vídeos em sequência

---

## Interface

<p align="center">
  <em>[ screenshots / demo em breve ]</em>
</p>

**Fluxo de uso:**

```
1. Selecionar vídeos
2. Ajustar região de facecam (opcional)
3. Configurar modo e parâmetros
4. Revisar e aprovar momentos detectados pela IA
5. Shorts gerados automaticamente com legenda
```

---

## Stack

| Camada | Tecnologia |
|---|---|
| Interface | CustomTkinter (Python) |
| Detecção de áudio | NumPy (análise RMS) |
| Detecção por IA | Gemini 2.5 Flash via Google AI Studio |
| Transcrição | OpenAI Whisper (modelo `small`) |
| Edição de vídeo | MoviePy v2.x |
| Legendas | Pillow (PIL) — sem ImageMagick |

---

## Status

![Em desenvolvimento](https://img.shields.io/badge/status-em%20desenvolvimento-blue)

Projeto em desenvolvimento ativo. Sendo usado em produção para criação de conteúdo de gaming.

---

## Contato

Desenvolvido por **William Ribeiro**
GitHub: [@UserM4C](https://github.com/UserM4C)

> Este repositório é um showcase. O código-fonte é proprietário.
