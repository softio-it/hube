# HUBE CDN

Arquivos de distribuição do HUBE para uso via JSDelivr.

> ⚠️ Este repositório contém **apenas builds de produção**.
> Código fonte: repositório privado.

---

## 📦 Uso via JSDelivr

### Latest (sempre a versão mais recente)

```html
<!-- Bundle Nuvemshop -->
<script src="https://cdn.jsdelivr.net/gh/softio-it/hube@latest/dist/bundle.nuvemshop.min.js"></script>
```

### Versão específica (recomendado para produção)

```html
<!-- Usando tag de versão -->
<script src="https://cdn.jsdelivr.net/gh/softio-it/hube@1.0.0/dist/bundle.nuvemshop.min.js"></script>

<!-- Usando commit hash -->
<script src="https://cdn.jsdelivr.net/gh/softio-it/hube@abc1234/dist/bundle.nuvemshop.min.js"></script>
```

---

## 🌐 URLs Disponíveis

### Bundles Principais (Bootstrap)

| Plataforma | URL |
|------------|-----|
| **Nuvemshop** | `https://cdn.jsdelivr.net/gh/softio-it/hube@latest/dist/bundle.nuvemshop.min.js` |
| **Shopify** | `https://cdn.jsdelivr.net/gh/softio-it/hube@latest/dist/bundle.shopify.min.js` |
| **Tray** | `https://cdn.jsdelivr.net/gh/softio-it/hube@latest/dist/bundle.tray.min.js` |

### Features (Carregadas Dinamicamente)

| Feature | URL |
|---------|-----|
| **SmartForms** (Nuvemshop) | `https://cdn.jsdelivr.net/gh/softio-it/hube@latest/dist/nuvemshop/smartforms.min.js` |

> 💡 As features são carregadas automaticamente pelo bundle principal. Você não precisa incluí-las manualmente.

---

## 🔄 Purge de Cache

Para forçar a atualização imediata do JSDelivr após um novo deploy:

### Via URL (navegador)
```
https://purge.jsdelivr.net/gh/softio-it/hube@latest/dist/bundle.nuvemshop.min.js
```

### Via cURL
```bash
curl https://purge.jsdelivr.net/gh/softio-it/hube@latest/dist/bundle.nuvemshop.min.js
```

### Purge em massa
```bash
# Todos os bundles
curl https://purge.jsdelivr.net/gh/softio-it/hube@latest/dist/bundle.*.min.js

# Todos os arquivos
curl https://purge.jsdelivr.net/gh/softio-it/hube@latest/dist/*
```

---

## 📊 Informações Técnicas

- **CDN**: JSDelivr (grátis, global, com cache)
- **Cache padrão**: 7 dias
- **Atualização**: ~2-5 minutos após novo commit
- **Compressão**: Brotli + Gzip automático
- **HTTP/2**: Suportado
- **HTTPS**: Sempre

---

## 🔖 Versionamento

Este repositório usa versionamento semântico via **Git tags**.

### Criar nova versão

```bash
# No repositório de produção (este)
git tag v1.0.0
git push origin v1.0.0
```

### Usar versão específica

```html
<script src="https://cdn.jsdelivr.net/gh/softio-it/hube@v1.0.0/dist/bundle.nuvemshop.min.js"></script>
```

### Listar versões disponíveis

- [Releases](https://github.com/softio-it/hube/releases)
- [Tags](https://github.com/softio-it/hube/tags)

---

## 📈 Estatísticas JSDelivr

Visualize estatísticas de uso em:

```
https://www.jsdelivr.com/package/gh/softio-it/hube
```

---

## ⚙️ Deploy

Este repositório é atualizado automaticamente via script no repositório privado.

**NÃO** faça commits manuais na pasta `dist/`. Todos os arquivos são gerados via build automatizado.

---

## 📝 Licença

Propriedade de Softio IT. Todos os direitos reservados.

---

**Última atualização**: Automática via GitHub Actions
**Repositório fonte**: Privado
