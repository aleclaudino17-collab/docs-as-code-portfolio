# Template: Documentação de API REST

> **Versão:** 1.0.0 | **Autor:** [Seu Nome] | **Base URL:** `https://api.exemplo.com/v1`

---

## Autenticação

Todas as requisições requerem um token Bearer no header:

```http
Authorization: Bearer {seu_token}
```

> [!WARNING]
> Nunca exponha seu token em repositórios públicos ou client-side não seguro.

---

## Endpoints

### GET /recurso

Retorna uma lista de recursos.

#### Parâmetros de Query

| Parâmetro | Tipo | Obrigatório | Descrição |
|:---|:---:|:---:|:---|
| `page` | integer | Não | Número da página (default: 1) |
| `limit` | integer | Não | Itens por página (default: 20, max: 100) |

#### Resposta (200 OK)

```json
{
  "data": [
    {
      "id": "uuid",
      "nome": "string",
      "status": "ativo"
    }
  ],
  "meta": {
    "page": 1,
    "total": 150
  }
}
```

#### Códigos de Erro

| Código | Descrição | Quando ocorre |
|:---|:---|:---|
| `400` | Bad Request | Parâmetros inválidos |
| `401` | Unauthorized | Token ausente ou inválido |
| `404` | Not Found | Recurso não encontrado |

---

## Exemplos de Uso

### cURL

```bash
curl -X GET "https://api.exemplo.com/v1/recurso?page=1&limit=10" \
  -H "Authorization: Bearer {token}"
```

### Python (Requests)

```python
import requests

response = requests.get(
    "https://api.exemplo.com/v1/recurso",
    headers={"Authorization": f"Bearer {token}"},
    params={"page": 1, "limit": 10}
)
data = response.json()
```

---

> **Documento preparado por:** [Seu Nome] | [Seu LinkedIn]
