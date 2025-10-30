# Quiz ODS

Aplicação Flask simples para um quiz sobre os Objetivos de Desenvolvimento Sustentável (ODS).

Descrição
---------
Este projeto é um pequeno questionário (quiz) construído com Flask. As perguntas estão em `questions.py` e as páginas HTML em `templates/`. O estilo visual está em `static/style.css`.

Requisitos
----------
- Python 3.8+
- Virtualenv recomendado

Instalação e execução (Windows / PowerShell)
-----------------------------------------
1. Crie e ative um ambiente virtual (recomendado):

```powershell
python -m venv .venv
. .venv\Scripts\Activate.ps1
```

2. Instale dependências (Flask):

```powershell
pip install --upgrade pip
pip install Flask
```

3. Execute a aplicação:

```powershell
python .\app.py
```

4. Abra no navegador em `http://127.0.0.1:5000/`.

Estrutura do projeto
--------------------
- `app.py` - Aplicação Flask e rotas.
- `questions.py` - Lista de perguntas, opções e respostas corretas.
- `templates/` - Templates Jinja2 (`index.html`, `quiz.html`, `result.html`).
- `static/style.css` - Estilos usados nas páginas.

Como editar perguntas
---------------------
Edite `questions.py`: cada entrada é um dicionário com as chaves `question`, `options` (lista) e `answer` (string com a opção correta).

Exemplo:

```python
{
	"question": "Qual ODS trata de Educação de Qualidade?",
	"options": ["ODS 2", "ODS 4", "ODS 8", "ODS 10"],
	"answer": "ODS 4",
}
```

Notas
-----
- Os templates usam classes definidas em `static/style.css`.
- Se encontrar erros de dependência, verifique se o ambiente virtual está ativado.

Licença
-------
Use conforme desejar — este é um exemplo educacional.
