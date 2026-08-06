# Aula 2 - Comandos Django

## Ativar o ambiente virtual

```powershell
venv\Scripts\Activate.ps1
```

### Para que serve?

Ativa o ambiente virtual (`venv`) do projeto.

Após executar, o terminal passa a mostrar:

```text
(venv)
```

Isso indica que todas as bibliotecas instaladas serão adicionadas apenas a esse projeto.

---

## Instalar dependências

```powershell
pip install django djangorestframework django-cors-headers
```

### Para que serve?

Instala as bibliotecas necessárias para o projeto.

- `django` → Framework web em Python.
- `djangorestframework` → Criação de APIs REST.
- `django-cors-headers` → Permite que aplicações Front-end (como React ou Vue) acessem a API sem problemas de CORS.

---

## Criar um projeto Django

```powershell
django-admin startproject loja .
```

### Para que serve?

Cria um novo projeto Django.

Neste exemplo:

- `django-admin` → Ferramenta de gerenciamento do Django.
- `startproject` → Comando para criar um projeto.
- `loja` → Nome do projeto.
- `.` → Cria o projeto na pasta atual, sem criar uma nova pasta chamada `loja`.

---

## Criar uma aplicação (App)

```powershell
python manage.py startapp produtos
```

### Para que serve?

Cria uma aplicação dentro do projeto Django.

Neste exemplo:

- `python` → Executa o interpretador Python.
- `manage.py` → Arquivo responsável por administrar o projeto Django.
- `startapp` → Cria uma nova aplicação.
- `produtos` → Nome da aplicação criada.

Após executar, será criada uma pasta semelhante a:

```text
produtos/
├── admin.py
├── apps.py
├── migrations/
├── models.py
├── tests.py
├── views.py
└── ...
```

Cada aplicação representa um módulo do sistema. Por exemplo:

- produtos
- clientes
- pedidos
- usuários

Cada uma possui seus próprios modelos, views e arquivos de configuração.

---