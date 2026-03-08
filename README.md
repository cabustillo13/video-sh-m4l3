# Model Context Protocol (MCP)

Este repositorio contiene 2 demos prácticas en video para la **Lecture 3 del Módulo 4**, donde se introduce el **Model Context Protocol (MCP)** y su uso para estandarizar la interacción entre aplicaciones y herramientas.

Las demos muestran:
* cómo MCP evita integraciones **ad-hoc**
* cómo funcionan las **primitivas principales del protocolo**

## Estructura
* `video-1-mcp-ad-hoc-vs-protocol/` : Ejemplo de múltiples aplicaciones (dashboard, Slack y web) llamando un mismo servidor MCP
* `video-2-mcp-primitives-demo/` : Exploración de primitivas MCP (tools y resources) desde un cliente

---

# Configuración

1. Crear y activar un entorno virtual.
    ```
    python -m venv .venv
    source .venv/bin/activate
    ```

    Windows PowerShell: `.venv\Scripts\activate`

2. Instalar dependencias.
    ```
    pip install -r requirements.txt
    ```

---

# Ejecución de las Demos

## Video 1: MCP Ad-hoc vs Protocol

Ir al directorio del video: `cd video-1-mcp-ad-hoc-vs-protocol/mcp_server`

Ejecutar los clientes que interactúan con el servidor MCP.

- Dashboard client: `python dashboard_client.py`
- Slack client: `python slack_client.py`
- Web client: `python web_client.py`

Cada cliente llama la misma herramienta (`create_ticket`) en el servidor MCP.

---

## Video 2: MCP Primitives

Ir al directorio del video:

```bash
cd video-2-mcp-primitives-demo
```

Ejecutar el cliente de demostración:

```bash
python client_demo.py
```

El cliente realiza las siguientes operaciones:

* lista las **tools** disponibles
* lista los **resources**
* llama la tool `create_refund_ticket`

---

# Resolución de Problemas

**ModuleNotFoundError**: Asegurarse de instalar las dependencias dentro del entorno virtual activado:

```
pip install -r requirements.txt
```