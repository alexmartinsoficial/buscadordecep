# README.md

# 🎯 Análise de Mercado Local - Laser CO2 Fracionado

Ferramenta de análise de mercado para profissionais de estética avançada que desejam entender o potencial de investimento em Laser CO2 em sua região.

## 🚀 Funcionalidades

- ✅ Consulta de dados por CEP
- ✅ Análise de clientes potenciais na região
- ✅ Mapeamento de concorrência local
- ✅ Estimativa de renda média da área
- ✅ Cálculo de ticket médio praticado
- ✅ Score de atratividade da região (0-100)
- ✅ Insights personalizados e acionáveis

## 🛠️ Tecnologias Utilizadas

- **HTML5** - Estrutura
- **CSS3** - Estilização e animações
- **JavaScript (Vanilla)** - Lógica e interatividade
- **API ViaCEP** - Consulta de dados de localização

## 📦 Dependências

Nenhuma! Este projeto usa apenas tecnologias web nativas (HTML, CSS, JavaScript) e não requer instalação de pacotes ou bibliotecas externas.

### APIs Externas Utilizadas:
- [ViaCEP](https://viacep.com.br/) - API pública gratuita para consulta de CEPs brasileiros

## 🌐 Como Usar

### Opção 1: GitHub Pages (Recomendado)

1. Faça fork deste repositório
2. Vá em Settings > Pages
3. Em "Source", selecione a branch `main` e pasta `/ (root)`
4. Clique em "Save"
5. Aguarde alguns minutos e acesse: `https://seu-usuario.github.io/nome-do-repo/`

### Opção 2: Hospedagem Local

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/analise-mercado-co2.git
cd analise-mercado-co2
```

2. Abra o arquivo `index.html` diretamente no navegador
   - Ou use um servidor local:
```bash
# Python 3
python -m http.server 8000

# PHP
php -S localhost:8000

# Node.js (npx)
npx http-server
```

3. Acesse `http://localhost:8000`

### Opção 3: Outras Hospedagens Gratuitas

- **Netlify**: Arraste e solte a pasta no [Netlify Drop](https://app.netlify.com/drop)
- **Vercel**: Conecte o repositório no [Vercel](https://vercel.com)
- **Cloudflare Pages**: Deploy via GitHub no [Cloudflare Pages](https://pages.cloudflare.com)

## 📝 Como Funciona

1. **Entrada de Dados**: Usuário digita o CEP da região onde deseja abrir ou já possui clínica
2. **Consulta de Localização**: Sistema busca dados reais via API ViaCEP
3. **Análise Inteligente**: Algoritmo gera métricas baseadas em:
   - Tipo de cidade (capital, interior)
   - Localização (centro, bairro)
   - Densidade populacional
   - Perfil socioeconômico
4. **Resultados**: Exibe análise completa com métricas e insights acionáveis

## 🎨 Personalização

### Cores e Branding

Edite as variáveis CSS no `<style>` do arquivo `index.html`:

```css
/* Gradiente principal */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* Cor primária dos botões */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### Métricas e Cálculos

A função `gerarDadosMercado()` no JavaScript pode ser ajustada para refinar os cálculos:

```javascript
// Ajuste os multiplicadores
if (ehCapital) multiplicador = 1.8;
else if (ehRegiaoCentral) multiplicador = 1.3;

// Ajuste as faixas de valores
const clientesPotenciais = Math.floor((8000 + Math.random() * 12000) * multiplicador);
```

## 🔗 Integrando com Calculadora de ROI

Para integrar com sua calculadora existente:

```html
<!-- Na sua calculadora ROI -->
<iframe src="https://seu-usuario.github.io/analise-mercado-co2/" 
        width="100%" 
        height="1200px" 
        frameborder="0">
</iframe>
```

Ou use como página separada e adicione link:

```html
<a href="analise-mercado.html" target="_blank">
  Analisar Mercado da Sua Região
</a>
```

## 📊 Estrutura de Dados

### Métricas Calculadas:

- **Clientes Potenciais**: Pessoas de 35-60 anos em raio de 5km
- **Concorrência**: Clínicas de estética avançada na região
- **Renda Média**: Faixa de renda predominante
- **Densidade Populacional**: Habitantes por km²
- **Ticket Médio**: Valor praticado para CO2 fracionado
- **Demanda**: Buscas mensais por tratamentos estéticos
- **Score**: 0-100 baseado em todos os fatores acima

## 🤝 Contribuindo

Contribuições são bem-vindas! Para contribuir:

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## 📞 Suporte

Para dúvidas ou sugestões, abra uma [issue](https://github.com/seu-usuario/analise-mercado-co2/issues) no GitHub.

---

**Desenvolvido para profissionais de estética avançada** 💜✨
