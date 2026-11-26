# Como atualizar o manual EVO

## Editar um slide

1. Abra [conteudo/slides.js](conteudo/slides.js) e procure pelo título.
2. Edite `description` para mudar o texto. Use `section` para escolher o grupo no índice.
3. Salve a alteração e confira o slide na prévia.

## Adicionar fotos

1. Envie os arquivos PNG, JPG ou WebP para uma pasta em `images/`, como `images/renovacao/`.
2. No slide, adicione os caminhos em `images`, na ordem de exibição.
3. Adicione os nomes correspondentes em `imageLabels`, na mesma ordem.

## Adicionar um slide

Copie um slide visual em `conteudo/slides.js` e cole antes do slide de encerramento, mantendo a vírgula entre os itens. Use este modelo:

```js
{
  "title": "NOVO PROCEDIMENTO",
  "section": "Contratos",
  "description": "Descreva o procedimento aqui.",
  "images": ["images/novo-procedimento/01-abertura.png"],
  "imageLabels": ["Abrir procedimento"],
  "pages": [],
  "type": "visual",
  "customSteps": true
}
```

O índice e a numeração acompanham a ordem dos slides nesse arquivo. Os caminhos das imagens começam na raiz do site, onde fica o `index.html`. As capturas atuais de contratos recorrentes são carregadas pelo arquivo `contratos-recorrentes.js`.
