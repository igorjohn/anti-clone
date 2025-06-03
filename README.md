# 🚫 Script Anti-Clonagem 

O objetivo desse script é **impedir** (ou, pelo menos, **dificultar consideravelmente**) que outras pessoas consigam **clonar** suas páginas e ofertas.

## 🚀 Funcionalidades

O script oferece várias camadas de proteção que podem ser ativadas/desativadas individualmente:

- **🛡️ Bloqueio de DevTools**: Impede a abertura das ferramentas de desenvolvimento do navegador
- **🔒 Bloqueio de Atalhos do Código Fonte**: Bloqueia atalhos de teclado que mostram o código fonte
- **🖱️ Bloqueio do Botão Direito**: Desativa o clique com botão direito
- **⌨️ Bloqueio de Atalhos**: Previne o uso de atalhos do teclado (Ctrl/Cmd)
- **📋 Bloqueio de Seleção de Texto**: Impede a seleção de texto na página
- **🧹 Deleta o código HTML**: Opção de deletar todo o HTML da página em caso de tentativa de violação
- **🔍 Verificação de Origem Facebook**: Opção para bloquear acesso direto sem o parâmetro "fbclid" na URL

## 📦 Como Usar

1. Copie o conteúdo do arquivo `index.html`
2. Cole em seu projeto
3. Personalize as configurações conforme necessário

## ⚙️ Configuração

As configurações podem ser ajustadas através do objeto `configOptions`:

```javascript
const configOptions = {
  blockDevTools: false,              // Bloquear DevTools
  blockSourceCodeShortcuts: false,   // Bloquear atalhos para código fonte
  blockRightClick: true,             // Bloquear clique direito
  blockCtrl: false,                  // Bloquear atalhos Ctrl/Cmd
  blockWhenDoesntHaveFbclid: false,  // Bloquear acesso sem fbclid
  blockTextSelection: true,          // Bloquear seleção de texto
  cleanHTML: true                    // Limpar HTML em caso de violação
}
```

## 🛠️ Personalização

O script inclui uma interface visual com switches para controlar todas as opções em tempo real. Para cada opção você pode:

1. Ativar/desativar através dos switches
2. Ver o status atual no painel de configuração
3. Copiar as configurações em formato JSON

## ⚠️ Observações Importantes

- O script deve ser incluído antes do fechamento da tag `</body>`
- Algumas funcionalidades podem ser afetadas por políticas de segurança do navegador
- Recomenda-se testar todas as configurações em diferentes navegadores

## 🤝 Contribuindo

Sinta-se à vontade para:
1. Fazer um fork do projeto
2. Criar uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abrir um Pull Request

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

---

⭐ Se este projeto te ajudou, considere dar uma estrela no GitHub! 