# Prompt para colar no Claude Code

Abra o Claude Code em qualquer pasta e cole o texto abaixo. Ele mesmo baixa o kit.

---

Quero montar meu requerimento de **Atividades Complementares** do IFNMG Campus Montes Claros e enviar num PDF único. Responda em português, tom direto.

**Passo 0 — baixar o kit.** Na minha pasta Documentos, rode `git clone https://github.com/Oikky/atividades-complementares-ifnmg` (se a pasta já existir, entre nela e rode `git pull`). Se não tiver git, baixe https://github.com/Oikky/atividades-complementares-ifnmg/archive/refs/heads/main.zip e extraia. Instale o que faltar para trabalhar com .docx e PDF (`pip install python-docx pypdf`). Trabalhe dentro dessa pasta e use estes arquivos:

- `MOLDE - Requerimento Atividades Complementares (Edificacoes Integrado).docx` — o formulário já formatado em .docx (Folha 1 + ANEXO 01 + ANEXO 02), em branco. Preencha com python-docx, sem mudar a estrutura.
- `Formulario original (em branco).doc` — modelo oficial, só para conferência.
- `REGRAS.md` — regras do PPC e a tabela de tetos por categoria.

**Antes de tudo, me pergunte:** nome completo, curso (o molde é de Técnico em Edificações **Integrado** = 90h; Concomitante/Subsequente exige 60h — se for outro curso, confira o PPC), período/ano, ano/semestre e onde estão meus certificados (pasta, zip, e-mail).

## O que fazer

1. **Achar os comprovantes.** Procure em Downloads, Documentos e na pasta que eu indicar (inclusive dentro de .zip) por PDFs/imagens de certificado. Fontes onde normalmente estão e onde eu posso baixar de novo:
   - Sistema de eventos do IFNMG (SIC, seminários, JIFENMG, etc.): https://eventos.ifnmg.edu.br/certificados — cada certificado tem um **token**; a página de validação do token mostra a **carga horária (CH)**, mesmo quando o PDF não mostra. Imprima essa validação em PDF e anexe junto.
   - Anais do SIC (artigos/resumos publicados): https://eventos.ifnmg.edu.br/sic2025/anais
   - Escola Virtual.Gov (EV.G): https://www.escolavirtual.gov.br → Meus Certificados. Validação por código em https://www.escolavirtual.gov.br/documentos/validacao (não tem URL direta; precisa digitar o código no formulário e salvar a página em PDF).
   - Even3, Cursa, SEI/IFNMG (bolsas PIBITI/PIBIC), Google Drive de professores.
   - Se não conseguir baixar sozinho (login, captcha), me diga o passo a passo e eu baixo manualmente. **Não mexa em login/senha nem copie perfil do navegador.**
2. **Ler cada comprovante** e anotar: atividade, datas de início/fim, CH, código/token de validação.
3. **Classificar** cada um numa categoria da tabela (`REGRAS.md`), respeitando o **teto** de cada categoria (conta a CH real até o teto). Mostre um placar com total e margem sobre 90h. Aponte os comprovantes fracos (sem CH, categoria duvidosa, datas estranhas, fora do período do curso) e **me deixe decidir** se entram.
4. **Preencher o molde**: Folha 1 (nome, curso, período, data), ANEXO 01 (coluna TOTAL por categoria + TOTAL geral; observação se precisar explicar algo, ex.: bolsa sem CH total declarada), ANEXO 02 (uma linha por comprovante, na ordem: item, atividade, ano, CH, comprovante com código/token, finalizado em). Salve como `REQUERIMENTO ATIVIDADES COMPLEMENTARES - <Nome> (preenchido).docx`.
5. **Renomear os comprovantes** numa pasta `Comprovantes/` como `01 - ...pdf`, `02 - ...pdf`… na mesma ordem do ANEXO 02 (validações como `01b - Validacao ...pdf`).
6. **Montar o PDF final** nesta ordem: Folha 1 (assinada) → ANEXO 01 → ANEXO 02 → comprovantes na ordem do ANEXO 02. Gere também `FOLHA 1 - imprimir e assinar.pdf` separado; eu imprimo, assino à mão, escaneio e você troca a pág. 1.
7. Escreva um `LEIA-ME.md` com placar, riscos e pendências.

**Não envie e-mail por mim.** O envio é meu, pelo meu e-mail, para **geraldo.vargas@ifnmg.edu.br**. Lembre que o requerimento só pode ser protocolado **uma vez por período letivo**, então tudo tem que estar junto antes.
