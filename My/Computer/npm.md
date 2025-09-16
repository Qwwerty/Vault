## 🧩 O que é `patch-package`?

O `patch-package` permite que você **modifique o código dentro do `node_modules`** e mantenha essas alterações mesmo após rodar `npm install` ou `yarn install`.

Sem ele, qualquer mudança que você fizesse manualmente no `node_modules` seria **apagada** na próxima instalação.

## 💡 Como funciona?

### Etapas básicas:

1. **Você edita manualmente** um arquivo dentro de `node_modules`.
    
2. Roda `npx patch-package nome-do-pacote`.
    
3. Ele cria um arquivo `.patch` em uma pasta chamada `patches/`.
    
4. Quando você roda `npm install`, o `patch-package` aplica automaticamente esses `.patches` nos pacotes modificados.