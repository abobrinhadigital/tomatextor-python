# 🎙️ Transcritor IA

Script Python para transcrição automática de arquivos de áudio utilizando **Faster-Whisper**. Otimizado para rodar localmente com aceleração por hardware (NVIDIA CUDA).

## ✨ Funcionalidades

* **Foco em MP3:** Processamento otimizado para arquivos `.mp3`.
* **Entrada e Saída Organizadas:** Áudios lidos da pasta `audios/` e transcrições salvas automaticamente na pasta `transcricoes/`, mantendo o código isolado.
* **Aceleração por GPU:** Utiliza núcleos CUDA para máxima velocidade.

## 🚀 Requisitos

* **Python 3.10+**: É necessário ter o Python instalado no sistema.
* **Drivers NVIDIA & CUDA**: Para aceleração por hardware na GPU.
* **FFmpeg**: Essencial para a decodificação de áudio.
* **Fish Shell**: O script auxiliar (`.sh`) é obrigatório para usuários deste shell.

### Instalação de dependências (Arch/CachyOS)

```bash
yay -S cuda cudnn ffmpeg
```

## 🛠️ Instalação

1. **Clone o repositório e acesse a pasta:**
```bash
git clone https://github.com/abobrinhadigital/transcritor-ia.git
cd transcritor-ia
```
2. **Crie e prepare o ambiente virtual:**
```fish
python -m venv venv
source venv/bin/activate.fish
pip install torch faster-whisper
```

## 📋 Como Usar

1. Coloque seus arquivos `.mp3` dentro da pasta `audios/`.
2. Execute o script via shell a partir da raiz do projeto:
```fish
chmod +x transcrever.sh
./transcrever.sh
```
