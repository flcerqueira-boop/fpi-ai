# FPI-AI — Foot Posture Index Fotográfico

> Ferramenta de análise fotográfica do Foot Posture Index baseada em visão computacional (Gemini AI).  
> Desenvolvida como protótipo de Iniciação Científica.

---

## Sobre o Projeto

O **FPI-AI** é um aplicativo web que utiliza inteligência artificial para auxiliar na avaliação postural do pé por meio de fotografias padronizadas, baseando-se nos critérios observacionais do **Foot Posture Index (FPI-6)**.

### Limitação metodológica importante

O item 1 do FPI-6 original — **palpação da cabeça do tálus** — requer contato manual e **não pode ser avaliado por fotografia**. Por isso, esta ferramenta avalia **5 dos 6 itens** do instrumento original, sendo tecnicamente uma versão fotográfica adaptada.

O objetivo da Iniciação Científica é justamente **validar essa versão fotográfica** contra o FPI-6 completo aplicado por fisioterapeuta experiente.

---

## Itens Avaliados

| Item | Descrição | Avaliável por foto |
|------|-----------|-------------------|
| 1 | Palpação da cabeça do tálus | ❌ Não — pontuado como 0 |
| 2 | Curvaturas supra/infra-maleolares | ✅ Sim |
| 3 | Posição do calcâneo no plano frontal | ✅ Sim |
| 4 | Proeminência da região talonavicular | ✅ Sim |
| 5 | Congruência do arco longitudinal medial | ✅ Sim |
| 6 | Abdução/adução do antepé | ✅ Sim |

---

## Como Usar

### 1. Obter API Key (gratuito)

1. Acesse [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
2. Faça login com sua conta Google
3. Clique em **Create API Key**
4. Copie a chave gerada

> ⚠️ **Nunca compartilhe sua API Key** em chats, e-mails ou repositórios públicos.

### 2. Acessar o app

Acesse via GitHub Pages:  
👉 `https://seuusuario.github.io/fpi-ai`

Ou abra o arquivo `index.html` diretamente no navegador.

### 3. Fotografar o pé

Siga o **Protocolo Fotográfico** descrito em [`PROTOCOLO.md`](PROTOCOLO.md).  
As marcações corporais são essenciais para a precisão da análise.

### 4. Realizar a análise

1. Cole sua API Key no campo indicado
2. Preencha os dados do paciente
3. Faça upload das 3 fotografias
4. Clique em **Analisar com IA**
5. Aguarde o resultado (5–15 segundos)

---

## Tecnologias Utilizadas

| Tecnologia | Função |
|-----------|--------|
| HTML / CSS / JavaScript | Interface do app |
| Gemini 1.5 Flash (Google AI) | Análise das imagens |
| GitHub Pages | Hospedagem gratuita |

---

## Estrutura do Repositório

```
fpi-ai/
├── index.html          # Aplicativo principal
├── README.md           # Este arquivo
├── PROTOCOLO.md        # Protocolo fotográfico padronizado
└── FICHA_COLETA.md     # Ficha de coleta para validação
```

---

## Contexto Acadêmico

Este protótipo foi desenvolvido como ponto de partida para um estudo de **validação de instrumento** no âmbito de Iniciação Científica, com o seguinte delineamento:

- **Fase 1:** Desenvolvimento e padronização do protocolo fotográfico
- **Fase 2:** Coleta de dados — FPI-6 manual (padrão-ouro) vs FPI-AI (método em teste)
- **Fase 3:** Análise estatística de concordância (ICC, Kappa de Cohen, Bland-Altman)
- **Fase 4:** Redação e submissão de artigo científico

---

## Contribuindo

Alunos participantes da IC podem contribuir com:

- Melhorias na interface
- Refinamento do prompt de análise
- Documentação e protocolo
- Relatório de bugs

Abra uma **Issue** ou envie um **Pull Request**.

---

## Licença

Uso acadêmico e de pesquisa. Cite o repositório em publicações derivadas.

---

## Contato

Projeto orientado por fisioterapeuta especialista em fisioterapia ortopédica e esportiva.  
Para dúvidas sobre o protocolo clínico, entre em contato com o orientador da IC.
