# msfconsole

Imagem Docker leve baseada em Alpine Linux com o Metasploit Framework (`msfconsole`) pré-configurado e pronto para uso.

## Visão Geral

Este projeto fornece um ambiente Docker minimalista para execução do Metasploit Framework sobre Alpine Linux. O objetivo é disponibilizar um container leve, portátil e fácil de implantar para profissionais de segurança, pesquisadores e ambientes de laboratório.

## Recursos

- Imagem baseada em Alpine Linux
- Metasploit Framework pré-instalado
- Tamanho otimizado do container
- Inicialização rápida
- Adequado para laboratórios, ambientes de testes e pesquisa em segurança
- Fácil integração com Docker e fluxos de trabalho containerizados

## Requisitos

- Docker 24+
- Acesso à internet (para atualizações e downloads de módulos, quando necessário)

## Pull Image

```bash
docker pull <your-image>
```

## Build Image

```bash
git clone https://github.com/<username>/msfconsole.git

cd msfconsole

docker build -t msfconsole .
```

## Run Container

Interactive shell:

```bash
docker run -it --rm msfconsole
```

Start directly with msfconsole:

```bash
docker run -it --rm msfconsole msfconsole
```

Run in detached mode:

```bash
docker run -d --name msfconsole msfconsole
```

Access the running container:

```bash
docker exec -it msfconsole sh
```

## Usage

Launch the Metasploit Framework:

```bash
msfconsole
```

Example:

```bash
msfconsole -q
```

## Container Structure

```text
.
├── Dockerfile
└── README.md
```

## Aviso de Segurança

Este projeto destina-se exclusivamente a avaliações de segurança autorizadas, pesquisas, treinamentos e ambientes de laboratório.

Os usuários são responsáveis por cumprir todas as leis, regulamentações e políticas organizacionais aplicáveis.

## Contribuição

Contribuições, issues e sugestões de melhorias são bem-vindas.

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Open a Pull Request

## Licença

Este repositório fornece apenas o ambiente de conteinerização.

O Metasploit Framework permanece sujeito à sua respectiva licença e termos de uso.

## Disclaimer

Este projeto não possui afiliação nem é endossado pelos criadores do Metasploit Framework. Todas as marcas registradas e direitos autorais pertencem aos seus respectivos proprietários.
