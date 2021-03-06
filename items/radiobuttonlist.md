---
layout: default
title: Radiobuttonlist
parent: Itens
nav_order: 70
has_children: false
---
# Radiobuttonlist
{: .no_toc }


Itens do tipo radiobuttonlist representam uma lista de botões dentre os quais o usuário pode selecionar apenas um.
{: .fs-6 .fw-300 }

<div class="code-example" markdown="1">

Exemplo:
           <input type="radio" id="01" name="Exemplo" value="sim"/>
           <label for="sim">Sim</label>
           <input type="radio" id="01" name="Exemplo" value="nao"/>
           <label for="nao">Não</label>

</div>

## Índice
{: .no_toc .text-delta }

1. TOC
{:toc}

---


## Propriedades Comuns

Itens do tipo `radiobuttonlist` aceitam as seguintes propriedades comuns de itens: `usetonameform`, `gotonext`, `usetomarkasrevisionpending` e `hidelabel`. [Clique aqui](commonproperties.md) para conhecê-las.

---

## Propriedades Básicas

Itens do tipo `radiobuttonlist` também aceitam propriedades básicas de itens. [Clique aqui](basicproperties.md) para conhecê-las.

---

## Propriedades de Banco de Dados

Pelo fato de persistirem informação em memória, itens do tipo `radiobuttonlist` também aceitam propriedades de banco de dados. [Clique aqui](databaseproperties.md) para conhecê-las.

---

## Radiobuttonlist - Exemplo 1

A tela abaixo revela um grupo de opções de meios de transporte dentre os quais o usuário pode selecionar um.

<div class="code-example" markdown="1">

  <form>
    <div> Meio de Transporte </div>
    <input type="radio" id="onibus" name="meioDeTransporte" value="onibus">
    <label for="onibus">Ônibus</label><br>
    <input type="radio" id="carro" name="meioDeTransporte" value="carro">
    <label for="carro">Carro</label><br>
    <input type="radio" id="outro" name="meioDeTransporte" value="outro">
    <label for="outro">Outro</label>
  </form>
  
</div>


```markdown
[
  {
    "id": 10,
    "type": "radiobuttonlist",
    "text": "Meio de Transporte",
    "VALUECol": "V.KEY5",
    "ownedDICTID": 10,
    "ownedDICTtablealias": "D"
  }
]
```

---

## Radiobuttonlist - Exemplo 2

A tela abaixo revela o mesmo `radiobuttonlist` do exemplo anterior, porém a propriedade `hidelabel` foi alterada para `true`.

<div class="code-example" markdown="1">

  <form>
    <input type="radio" id="onibus" name="meioDeTransporte" value="onibus">
    <label for="onibus">Ônibus</label><br>
    <input type="radio" id="carro" name="meioDeTransporte" value="carro">
    <label for="carro">Carro</label><br>
    <input type="radio" id="outro" name="meioDeTransporte" value="outro">
    <label for="outro">Outro</label>
  </form>
  
</div>

```markdown
[
  {
    "id": 10,
    "type": "radiobuttonlist",
    "text": "Meio de Transporte",
    "VALUECol": "V.KEY5",
    "ownedDICTID": 10,
    "ownedDICTtablealias": "D",
    "hidelabel": true
  }
]
```
