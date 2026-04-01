# Token Efficiency

Uma habilidade que ensina agentes de programação a minimizar o desperdício de tokens em todas as operações de uso de ferramentas, leitura de arquivos e processamento de dados.

Cada byte de saída de uma ferramenta custa dinheiro e ocupa espaço na janela de contexto. Essa habilidade incentiva o hábito de filtrar, projetar e truncar na origem — em vez de despejar saídas brutas e torcer para o melhor.

> **Aviso de desativação:** Esta habilidade existe porque agentes atuais ainda não internalizaram o uso eficiente de ferramentas. À medida que os modelos melhorarem e essas práticas se tornarem padrão, esta habilidade será descontinuada.

## O que ela aborda

- Ferramentas de consulta estruturada (`jq`, `yq`, `awk`) em vez de despejar tudo e depois ler  
- Pesquisa precisa (`ast-grep`, `rg`) em vez de buscas de texto amplas  
- Fluxos de trabalho orientados a resumo no Git (`--stat`, `--name-only`)  
- Supressão de ruído de saída (flags silenciosas, `NO_COLOR`, leituras seletivas)  
- Detecção de mudanças baseada em *hash* em vez de reler arquivos  
- Uso de coreutils em vez de Python para transformações simples  

## Instalação

### Claude Code

Primeiro, adicione o marketplace:
```
/plugin marketplace add undefdev/token-efficiency
```

Depois instale:
```
/plugin install token-efficiency@undefdev-token-efficiency
```

### Cursor

Ainda não disponível no Cursor Marketplace. Por enquanto, clone o repositório e adicione o conteúdo da habilidade às regras do seu projeto manualmente.

### Gemini CLI

```bash
gemini extensions install https://github.com/undefdev/token-efficiency
```

### Codex

Consulte [.codex/INSTALL.md](.codex/INSTALL.md)

### OpenCode

Consulte [.opencode/INSTALL.md](.opencode/INSTALL.md)
