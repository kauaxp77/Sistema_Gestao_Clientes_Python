<p align="center">
  <img src="docs/banner.png" alt="Sistema de Gestão de Clientes" width="100%">
</p>

<h1 align="center">🗂️ Sistema de Gestão de Clientes</h1>

<p align="center">
  Aplicativo desktop em Python para o <b>cadastro rápido de clientes</b>: um formulário com interface moderna
  (temas claro e escuro) que grava cada ficha em uma <b>planilha Excel</b>.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/CustomTkinter-GUI-1f6aa5?style=for-the-badge" alt="CustomTkinter">
  <img src="https://img.shields.io/badge/openpyxl-Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" alt="openpyxl">
</p>

<p align="center">
  <a href="#-sobre-o-projeto">Sobre</a> •
  <a href="#-funcionalidades">Funcionalidades</a> •
  <a href="#️-telas">Telas</a> •
  <a href="#-como-executar">Como executar</a> •
  <a href="#-estrutura-do-projeto">Estrutura</a> •
  <a href="#️-tecnologias">Tecnologias</a>
</p>

---

## 📌 Sobre o projeto

Um sistema simples para quem precisa registrar clientes sem montar um banco de dados: o próprio arquivo
`clientes.xlsx` funciona como base. Na primeira execução o programa cria a planilha com o cabeçalho; a cada
cadastro salvo, uma nova linha é adicionada. Depois é só abrir o arquivo no Excel, LibreOffice ou Google Planilhas.

## ✨ Funcionalidades

| | Recurso | Descrição |
|---|---|---|
| 📝 | **Formulário de cadastro** | Nome completo, contato, idade, endereço, gênero e observações |
| ⚠️ | **Validação** | Se nome, contato, idade ou endereço estiverem vazios, mostra um aviso e não salva |
| 📊 | **Planilha Excel** | Cada cadastro vira uma linha em `clientes.xlsx`, criado automaticamente com o cabeçalho |
| 🧹 | **Limpar dados** | Esvazia os campos para o próximo cadastro |
| 🌗 | **Temas** | Light, Dark ou System (segue o tema do sistema operacional) |

## 🖼️ Telas

<table>
  <tr>
    <td align="center"><b>Tema claro</b><br><img src="docs/screenshots/formulario_claro.png" alt="Formulário no tema claro"></td>
    <td align="center"><b>Tema escuro</b><br><img src="docs/screenshots/formulario_escuro.png" alt="Formulário no tema escuro"></td>
  </tr>
  <tr>
    <td align="center" colspan="2"><b>Planilha gerada</b> (conteúdo do <code>clientes.xlsx</code> após dois cadastros de teste, com dados fictícios)<br><img src="docs/screenshots/planilha.png" alt="Planilha clientes.xlsx"></td>
  </tr>
</table>

## 🚀 Como executar

**Pré-requisito:** Python 3 com Tkinter (no Linux, pacote `python3-tk`).

```bash
git clone https://github.com/kauaxp77/Sistema_Gestao_Clientes_Python.git
cd Sistema_Gestao_Clientes_Python
pip install -r requirements.txt
python app.py
```

O arquivo `clientes.xlsx` é criado na pasta de onde o programa é executado.

> 🔒 A planilha guarda dados pessoais dos clientes e por isso está no `.gitignore`: ela fica só no computador
> de quem usa o sistema e não deve ser enviada ao repositório.

## 📁 Estrutura do projeto

```
Sistema_Gestao_Clientes_Python/
├── app.py             # Interface (CustomTkinter) e gravação na planilha (openpyxl)
├── requirements.txt   # customtkinter e openpyxl
└── docs/
    ├── banner.png
    └── screenshots/   # Capturas de tela usadas neste README
```

## 🛠️ Tecnologias

- **Python 3**: linguagem principal
- **CustomTkinter**: interface gráfica moderna, com temas claro e escuro
- **openpyxl**: criação e escrita da planilha `.xlsx`
- **Tkinter (messagebox)**: mensagens de erro e de sucesso

## 👨‍💻 Autor

Desenvolvido por **[kauaxp77](https://github.com/kauaxp77)**

<p align="center">⭐ Se curtiu o projeto, deixe uma estrela!</p>
