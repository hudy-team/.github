<div align="center">

# HuDy (휴디)

**대한민국 공휴일 API 서비스**

[![Website](https://img.shields.io/badge/Website-hudy.co.kr-E34234?style=for-the-badge&logo=google-chrome&logoColor=white)](https://www.hudy.co.kr)
[![npm](https://img.shields.io/npm/v/@hudy-sdk/sdk?style=for-the-badge&logo=npm&logoColor=white&label=SDK)](https://www.npmjs.com/package/@hudy-sdk/sdk)
[![PyPI](https://img.shields.io/pypi/v/hudy-sdk?style=for-the-badge&logo=pypi&logoColor=white&label=SDK)](https://pypi.org/project/hudy-sdk/)

<br/>

공휴일 조회 · 영업일 계산 · 커스텀 공휴일 · MCP 서버

한 줄의 API 호출로 대한민국 공휴일 데이터를 통합하세요.

</div>

<br/>

## Repositories

| Repository | Description | Stack |
|:-----------|:------------|:------|
| **[hudy_api_server](https://github.com/hudy-team/hudy_api_server)** | REST API 서버 | ![Rust](https://img.shields.io/badge/Rust-f74c00?logo=rust&logoColor=white) ![actix-web](https://img.shields.io/badge/actix--web-0055aa?logo=rust&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white) |
| **[hudy_frontend](https://github.com/hudy-team/hudy_frontend)** | 랜딩 페이지 + 대시보드 | ![Next.js](https://img.shields.io/badge/Next.js_16-000000?logo=next.js&logoColor=white) ![React](https://img.shields.io/badge/React_19-61DAFB?logo=react&logoColor=black) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white) |
| **[hudy_sdk](https://github.com/hudy-team/hudy_sdk)** | 공식 SDK (TypeScript + Python) | ![npm](https://img.shields.io/badge/npm-CB3837?logo=npm&logoColor=white) ![PyPI](https://img.shields.io/badge/PyPI-3775A9?logo=pypi&logoColor=white) |

<br/>

## Quick Start

### TypeScript / JavaScript

```bash
npm install @hudy-sdk/sdk
```

```typescript
import { HudyClient } from '@hudy-sdk/sdk';

const client = new HudyClient({ apiKey: 'hd_live_...' });
const holidays = await client.getHolidays(2025);
```

### Python

```bash
pip install hudy-sdk
```

```python
from hudy import HudyClient

client = HudyClient(api_key="hd_live_...")
holidays = client.get_holidays(2025)
```

### REST API

```bash
curl -H "x-api-key: <your-api-key>" \
  "https://api.hudy.co.kr/v1/holidays?year=2025"
```

<br/>

<div align="center">

**[홈페이지](https://www.hudy.co.kr)** · **[API 문서](https://www.hudy.co.kr/#docs)** · **[SDK 문서](https://github.com/hudy-team/hudy_sdk)**

</div>
