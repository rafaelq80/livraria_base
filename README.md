# Projeto Livraria

<br />

<div align="center">
    <img src="https://i.imgur.com/w8tTOuT.png" title="source: imgur.com" /> 
</div>
<br /><br />

## Diagrama de Classes

```mermaid
classDiagram
class Produto {
  - id : Long
  - titulo : String
  - autor: String
  - sinopse: String
  - editora: String
  - preco : BigDecimal
  - usuario : Usuario
  + getAll()
  + getById(Long id)
  + getByTitulo(String titulo)
  + post(Produto produto)
  + put(Produto produto)
  + deleteTema(Long id)
}
class Usuario {
  - id : Long
  - nome : String
  - usuario : String
  - senha : String
  - foto : String
  - produto : List ~Produto~
  + getAll()
  + getById(Long id)
  + autenticar(UsuarioLogin usuarioLogin)
  + cadastrar(Usuario usuario)
  + atualizar(Usuario usuario)
}
class UsuarioLogin{
  - id : Long
  - nome : String
  - usuario : String
  - senha : String
  - foto : String
  - token : String
}
Usuario --> Produto
```

<br /><br />

# Referências sobre Spring

<br />

<a href="https://spring.io/" target="_blank">Documentação Oficial do Spring</a>

<a href="https://maven.apache.org/" target="_blank">Documentação Oficial do Maven</a>

<a href="https://mvnrepository.com/" target="_blank">Repositório do Maven</a>

<a href="https://www.baeldung.com/" target="_blank">Baeldung</a>

<a href="https://blog.algaworks.com/" target="_blank">Blog da Algaworks</a>

<a href="https://www.michellibrito.com/" target="_blank">Michelli Brito</a>
