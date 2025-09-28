# Hugging Face para Visão Computacional

## Descrição
Este repositório apresenta um material didático sobre o uso do **Hugging Face** aplicado à **Visão Computacional**, com exemplos práticos em Python no Google Colab.  
O foco é mostrar como utilizar modelos pré-treinados para **classificação de imagens** e **detecção de objetos**, tanto de forma local quanto via **Inference API**.

---

## Estrutura do Repositório
```
huggingface-visao/
│
├── notebooks/
│   └── huggingface_visao_colab_final.ipynb
│
├── datasets/
│   └── imagens/     # imagens para teste
│
└── README.md
```

---

## Conteúdo do Notebook

1. **Instalação das dependências**  
2. **Login no Hugging Face Hub** (via *secrets* do Colab)  
3. **Preparação das imagens** (pasta `datasets/imagens/`)  
4. **Classificação de imagens** usando `google/vit-base-patch16-224`  
   - Exibição com `cv2_imshow`  
   - Resultados textuais das classes e scores  
5. **Detecção de objetos** usando `facebook/detr-resnet-50`  
   - Exibição com bounding boxes em **cores variadas**  
   - Impressão dos resultados detalhados  
6. **Uso da Inference API**  
   - Envio de imagens para classificação  
   - Envio de imagens para detecção, com visualização das caixas

---

## Como usar no Google Colab

1. **Clonar o repositório** ou enviar os notebooks.  
2. **Criar a pasta de imagens**:  
   ```bash
   !mkdir -p datasets/imagens
   ```
3. **Adicionar uma imagem de teste** na pasta `datasets/imagens/` (exemplo: `person.jpg`).  
4. **Habilitar GPU**:  
   - Menu → Ambiente de execução → Alterar tipo de ambiente de execução → GPU.  
5. Executar o notebook `huggingface_visao_colab_final.ipynb`.

---

## Referências e Fontes de Pesquisa
- [Documentação Hugging Face Hub](https://huggingface.co/docs/huggingface_hub)  
- [Transformers para Visão Computacional](https://huggingface.co/docs/transformers/tasks/image_classification)  
- [Modelos DETR (Facebook)](https://huggingface.co/facebook/detr-resnet-50)  
- [Modelos ViT (Google)](https://huggingface.co/google/vit-base-patch16-224)  
- Conteúdos organizados com apoio do **ChatGPT**  

---

## Sobre o repositório
Este repositório foi criado como **material de apoio didático** em aulas de Visão Computacional, destacando como explorar a integração de modelos de código aberto do Hugging Face em notebooks práticos.
