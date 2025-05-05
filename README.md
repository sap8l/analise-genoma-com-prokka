# analise-genoma-com-prokka
Protocolo para instalação e uso do Prokka para anotação genômica.
---

## 📌 O que é o Prokka?

Prokka é uma ferramenta de linha de comando que realiza a **anotação automática de genomas bacterianos**, gerando arquivos como `.gff`, `.gbk`, `.faa`, entre outros.

Repositório oficial: [https://github.com/tseemann/prokka](https://github.com/tseemann/prokka)

---

## 📥 Instalação

### ✅ Requisitos
- Linux, macOS ou WSL (Windows Subsystem for Linux)
- Miniconda ou Conda (recomendado)

### 🔧 Instalação via Conda (recomendado)
```bash
conda install -c bioconda prokka
```
## ▶️ Como usar o Prokka

Suponha que você tenha um arquivo FASTA chamado `meu_genoma.fasta`.

### ⚙️ Comando básico:
```bash
prokka meu_genoma.fasta --outdir anotacao --prefix resultado
```
## 🔍 Explicação dos parâmetros:


Parâmetro	Descrição


meu_genoma.fasta	Arquivo FASTA do genoma que será anotado


--outdir anotacao	Diretório onde os arquivos de saída serão salvos


--prefix resultado	Prefixo dos arquivos de saída gerados pelo Prokka

## 📁 Arquivos gerados na saída

O Prokka gera diversos arquivos úteis. Veja abaixo os principais e seus significados:

| Arquivo         | Descrição                                  |
| --------------- | ------------------------------------------ |
| `amostra01.gff` | Anotação geral no formato GFF              |
| `amostra01.gbk` | Arquivo anotado no formato GenBank         |
| `amostra01.faa` | Sequência de proteínas anotadas            |
| `amostra01.ffn` | Sequência de DNA dos genes codificantes    |
| `amostra01.fna` | Sequência genômica com headers atualizados |
| `amostra01.tsv` | Tabela com resumo das anotações            |
| `log.txt`       | Log do processo de execução do Prokka      |

