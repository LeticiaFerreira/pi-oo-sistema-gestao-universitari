# pi-sistema-gestao-universitario  
**Disciplina:** Desenvolvimento de Sistemas Orientado a Objetos  
**Instituição:** SENAC  
**Professor:** Enoque Felipe dos Santos Leal  

---

## Integrantes  
- Eduardo Dorea De Oliveira Macario Muniz  
- Guilherme Stark  
- Alexandre de Souza Sol  
- Leticia Silva Ferreira  
- Maria Adelia Sena de Lucena  
- Rodrigo Pinto do Amaral Lopes  
- Carlos Raphael Nunes Albuquerque  
- João Ricardo Vano Ferreira  

---

## Objetivo do Projeto  
Desenvolver um sistema orientado a objetos para **gestão de dados de uma universidade**, com foco em cadastros de diferentes perfis de usuários: alunos, professores, fornecedores, pessoas físicas e pessoas jurídicas.  

O projeto está dividido em fases:  
1. **Fase 1:** Modelagem UML (diagramas de caso de uso, classes e descrição de cenários).  
2. **Fase 2:** Protótipos funcionais das interfaces, de acordo com os diagramas da Fase 1.  

---

## Diagramas UML (Fase 1)  
### Diagrama de Caso de Uso
<img src="imagens/diagrama_caso_de_uso.png" alt="Diagrama Caso de Uso" width="400"/>

### Cenários de Cadastro
#### Pessoa Física  
- **Principal:** Administrador cadastra Nome, CPF, Data de Nascimento e Endereço → sistema valida CPF → salva dados.  
- **Alternativos:** CPF já cadastrado, CPF inválido, dados incompletos.  
- **Pré-condição:** Administrador logado.  
- **Pós-condição:** Pessoa Física registrada e disponível para associação a alunos/professores.  

#### Pessoa Jurídica  
- **Principal:** Administrador cadastra CNPJ, Razão Social, Endereço, Tipo de Serviço → sistema valida CNPJ → salva dados.  
- **Alternativos:** CNPJ já cadastrado, CPF inválido, dados incompletos.  
- **Pré-condição:** Administrador logado.  
- **Pós-condição:** Pessoa Jurídica vinculada ao sistema.  

#### Professor  
- **Principal:** Secretaria cadastra Matrícula, Departamento, Titulação, Salário → sistema associa a Pessoa Física existente.  
- **Alternativos:** Matrícula duplicada, Pessoa Física não cadastrada.  
- **Pré-condição:** Pessoa Física cadastrada.  
- **Pós-condição:** Professor recebe acesso ao sistema acadêmico.  

#### Aluno  
- **Principal:** Secretaria cadastra Matrícula, Curso, Período, Turno → sistema associa a Pessoa Física e gera e-mail institucional.  
- **Alternativos:** Curso sem vagas, dados inconsistentes.  
- **Pré-condição:** Pessoa Física cadastrada.  
- **Pós-condição:** Aluno recebe acesso ao portal acadêmico.  

#### Fornecedor  
- **Principal:** Secretaria cadastra Tipo de Fornecimento e CNPJ → sistema valida e salva dados.  
- **Alternativos:** CNPJ não cadastrado, pendência financeira.  
- **Pré-condição:** Pessoa Jurídica cadastrada.  
- **Pós-condição:** Fornecedor incluído no sistema de compras.  

### Diagrama de Classes  
<img src="imagens/diagrama_classes.png" alt="Diagrama de Classes" width="400"/>

---

## Protótipos (Fase 2)  
Os protótipos foram desenvolvidos no **Figma**, refletindo os cenários principais e alternativos da Fase 1.  

Acesse todos os protótipos aqui: [Protótipos no Figma](https://miro.com/app/board/uXjVJMVUzZ4=/?moveToWidget=3458764639411856994&cot=10)  

### Telas de Cadastro
- Pessoa Física  
<img src="imagens/cadastr-pessoa-fisica.jpg" alt="Cadastro Pessoa Física" width="400"/>  

- Pessoa Jurídica  
<img src="imagens/cadastro-pessoa-juridica.jpg" alt="Cadastro Pessoa Jurídica" width="400"/>  

- Professor  
<img src="imagens/cadastro-professor.jpg" alt="Cadastro Professor" width="400"/>  

- Aluno  
<img src="imagens/cadastro-aluno.jpg" alt="Cadastro Aluno" width="400"/>  

- Fornecedor  
<img src="imagens/cadastro-fornecedor.jpg" alt="Cadastro Fornecedor" width="400"/>  

### Telas do Sistema
- Tela Inicial  
<img src="imagens/tela-inicial.jpg" alt="Tela Inicial" width="400"/>  

- Sistema Universidade - Secretaria  
<img src="imagens/sistema-universidade-secretaria.jpg" alt="Sistema Universidade - Secretaria" width="400"/>  

- Sistema Universidade - Administrador  
<img src="imagens/sistema-universidade-adm.jpg" alt="Sistema Universidade - ADM" width="400"/>  

- Login  
<img src="imagens/login.jpg" alt="Login" width="400"/>  

### Mensagens e Erros
- Cadastro Realizado  
<img src="imagens/mensagem-cadastro-realizado.jpg" alt="Mensagem Cadastro Realizado" width="400"/>  

- CPF Inválido  
<img src="imagens/mensagem-cpf.jpg" alt="Mensagem CPF" width="400"/>  
<img src="imagens/mensagem-cpf-2.jpg" alt="Mensagem CPF 2" width="400"/>  

- Dados Incompletos  
<img src="imagens/mensagem-dados-incompletos.jpg" alt="Mensagem Dados Incompletos" width="400"/>

- Cadastro Realizado Professor
<img src= "imagens/mensagem-cadastro-professor.jpg" alt="Mensagem Cadastro Professor" width="400"/>
  
- Cadastro Realizado Aluno
<img src= "imagens/mensagem-cadastro-aluno.jpg" alt="Mensagem Cadastro aluno" width="400"/>

- Cadastro Realizado Fornecedor 
<img src= "imagens/mensagem-cadastro-fornecedor.jpg" alt="Mensagem Cadastro Fornecedor" width="400"/>

- Erro Cadastrado  
<img src="imagens/erro-cadastrado.jpg" alt="Erro Cadastrado" width="400"/>  

- Erro Inválido  
<img src="imagens/erro-invalido.jpg" alt="Erro Inválido" width="400"/>
 
- Erro Duplicidade
<img src="imagens/erro-matrícula-professor.jpg"  alt="Erro Duplicidade" width="400"/>

- Erro Dados
<img src="imagens/erro-dados-aluno.jpg" alt="Erro Dados" width="400"/>

- Erro Pessoa Física
<img src="imagens/erro-pessoafísica-professor.jpg" alt="Erro Pessoa Física" width="400"/>
 
- Erro sem vagas
<img src="imagens/erro-vagas-aluno.jpg" alt="Erro sem vagas" width="400" />

- Erro Pessoa Jurídica
<img src="imagens/erro-pessoajurídica-fornecedor.jpg"  alt="Erro Pessoa Jurídica" width="400"/>

- Erro Pendências
<img src="imagens/erro-pendências-fornecedor.jpg" alt="Erro Pendências" width="400"/>

### Telas Auxiliares

- Lista de espera
<img src="imagens/lista-de-espera-vagas-aluno.jpg" alt="Lista de Espera Vagas Aluno" width="400"/>

- Revisão de Dados
<img src="imagens/revisão-dados-aluno.jpg" alt="Revisao Dados Aluno" width="400"/>

- Pendências Financeiras
<img src="imagens/pendências-fornecedor.jpg" alt="Pendências Fornecedor" width="400"/> 


 
  
---

## Estrutura do Repositório  
/pi-sistema-gestao-universitario  
├── imagens/ # Diagramas e prints dos protótipos  
├── README.md # Documentação principal do projeto  

---

## Referências  
- [Guia definitivo para diagramas UML](https://miro.com/pt/diagrama/o-que-e-uml/)  
- COSTA, M. A. S. *Modelagem de um sistema acadêmico baseado em UML para universidades federais*. Dissertação (Mestrado em Ciência da Computação) – UFMG, 2021. Disponível em: https://repositorio.ufmg.br/handle/1843/36789
