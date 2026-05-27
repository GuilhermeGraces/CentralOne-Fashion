# CentralOne Fashion

> *Sistema corporativo de gestão para lojas de roupas e acessórios*

![.NET](https://img.shields.io/badge/.NET-10-purple)
![SQLite](https://img.shields.io/badge/Database-SQLite-green)
![Swagger](https://img.shields.io/badge/API-Swagger-brightgreen)
![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)

---

## Descrição do Sistema

O **CentralOne Fashion** é uma plataforma corporativa desenvolvida para lojas de roupas e acessórios que precisam centralizar e automatizar sua gestão diária.

O sistema foi criado para resolver um problema comum no varejo de moda: a dificuldade em controlar vendas, estoque e finanças de forma integrada em um único ambiente.

Gerentes, vendedores e administradores de lojas utilizam a plataforma para acompanhar em tempo real os indicadores do negócio, registrar vendas, controlar entradas e saídas de mercadorias e gerar relatórios gerenciais.

A solução oferece uma interface moderna, responsiva e intuitiva, eliminando o uso de planilhas manuais e sistemas desconectados.

Com o **CentralOne Fashion**, o lojista ganha mais organização, produtividade e eficiência na administração do negócio, podendo tomar decisões baseadas em dados concretos.

---

## Tecnologias Utilizadas

| Tecnologia | Finalidade |
|---|---|
| C# | Linguagem principal de desenvolvimento |
| ASP.NET Core .NET 10 | Framework backend e MVC |
| Entity Framework Core 10 | ORM para acesso ao banco de dados |
| SQLite | Banco de dados local |
| Bootstrap 5 | Interface responsiva |
| Swagger / OpenAPI | Documentação e testes da API REST |

---

## Estrutura de Pastas

```txt
CentralOneFashion/
│
├── src/                          # Código-fonte principal da aplicação
│   ├── CentralOneFashion.API/    # Endpoints REST e documentação Swagger
│   ├── CentralOneFashion.Web/    # Interface MVC administrativa
│   ├── CentralOneFashion.Core/   # Entidades e regras de domínio
│   └── CentralOneFashion.Application/ # Serviços, casos de uso e validações
│
├── docs/                         # Documentação técnica do projeto
│   ├── arquitetura.md
│   └── endpoints.md
│
├── tests/                        # Testes automatizados
│   └── CentralOneFashion.Tests/
│
└── CentralOneFashion.sln         # Arquivo de solução .NET
```

- **src/** — contém todo o código-fonte dividido em camadas (API, Web, Core e Application)
- **docs/** — reúne a documentação técnica, diagramas e especificações do sistema
- **tests/** — contém os projetos de testes unitários e de integração

---

## Principais Funcionalidades

- **Dashboard administrativo** com indicadores operacionais em tempo real
- **Cadastro de produtos** com controle de tamanhos, cores, preços e imagens
- **Controle de estoque** com alertas de quantidade mínima
- **Gestão de vendas** com múltiplas formas de pagamento e emissão de comprovantes
- **Cadastro de clientes** com histórico de compras
- **Controle financeiro** com faturamento diário e mensal
- **Relatórios gerenciais** por período e por produto
- **API REST** documentada via Swagger

---

## Como Executar o Projeto

### Pré-requisitos

- [.NET SDK 10](https://dotnet.microsoft.com/download)
- Visual Studio 2022 ou VS Code

### 1. Clonar o repositório

```bash
git clone https://github.com/centralonetech/centralone-fashion.git
cd centralone-fashion
```

### 2. Restaurar dependências

```bash
dotnet restore
```

### 3. Executar a API

```bash
cd src/CentralOneFashion.API
dotnet run --urls="http://localhost:7001"
```

Acesse a documentação Swagger em:

```
http://localhost:7001/swagger
```

### 4. Executar o Frontend Web

Abra um novo terminal e execute:

```bash
cd src/CentralOneFashion.Web
dotnet run --urls="http://localhost:5090"
```

Acesse o sistema em:

```
http://localhost:5090
```

---

## Exemplos de Uso da API

### Listar todos os produtos

```http
GET /api/produtos
```

### Buscar produto por ID

```http
GET /api/produtos/{id}
```

### Cadastrar novo produto

```http
POST /api/produtos
Content-Type: application/json

{
  "nome": "Camiseta Oversized",
  "categoria": "Moda Masculina",
  "preco": 89.90,
  "estoque": 25
}
```

---

## Fluxo do Sistema

```
Usuário → Frontend MVC → Controllers → Application Services → API REST → Entity Framework Core → SQLite
```

---

## Links

- 🌐 [Site da empresa](https://www.centralonetech.com.br)
- 📁 [Repositório no GitHub](https://github.com/centralonetech/centralone-fashion)
- 📖 [Documentação da API](http://localhost:7001/swagger)

---

## Melhorias Futuras

- *Integração com meios de pagamento online*
- *Emissão de notas fiscais eletrônicas*
- *Autenticação JWT e controle de permissões*
- *Dashboard analítico avançado com gráficos*
- *Integração com WhatsApp para notificações*
- *Suporte a múltiplas filiais*
- *Aplicativo mobile*

---

## Licença

Projeto acadêmico desenvolvido para fins educacionais — **CentralOne Tech** © 2025


---


### Alunos:

- *Marcos Portales Cruz - 114.017*

- *ENZO Musskopf Lupinetti - 114.019*

- *Kaemy dos Reis Moreira - 114.032*

- *Khristofer Dambrozo Maciel - 114.107*

- *Carlos Eduardo Mascarenhas de Oliveira - 114.007*

