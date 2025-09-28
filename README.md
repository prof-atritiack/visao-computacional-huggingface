# Hugging Face para Visão Computacional

## Descrição
Este repositório apresenta um material didático sobre o uso do **Hugging Face** aplicado à **Visão Computacional**, com exemplos práticos no Google Colab.  
O notebook demonstra como realizar **classificação de imagens** e **detecção de objetos** utilizando modelos pré-treinados, além do uso da **Inference API**.

---

## Estrutura do Repositório
```
huggingface-visao/
│
├── notebooks/
│   └── huggingface_visao_colab_padronizado.ipynb
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
3. **Preparação das imagens de teste** (pasta `datasets/imagens/`)  
4. **Classificação de imagens** com `google/vit-base-patch16-224`  
   - Visualização com `cv2_imshow`  
   - Impressão das classes e scores  
5. **Detecção de objetos** com `facebook/detr-resnet-50`  
   - Bounding boxes em **cores variadas**  
   - Impressão dos resultados  
6. **Uso da Inference API**  
   - Classificação via API  
   - Detecção de objetos via API (com visualização das caixas)

---

## Como usar no Google Colab

1. **Criar a pasta de imagens**:  
   ```bash
   !mkdir -p datasets/imagens
   ```
2. **Adicionar uma imagem de teste** em `datasets/imagens/` (exemplo: `exemplo.jpg`).  
3. **Configurar o token** do Hugging Face nos *secrets* do Colab (`HF_TOKEN`).  
4. **Habilitar GPU**:  
   - Menu → Ambiente de execução → Alterar tipo de ambiente de execução → GPU.  
5. Executar o notebook `huggingface_visao_colab_padronizado.ipynb`.

---

## Referências e Fontes de Pesquisa
- [Documentação Hugging Face Hub](https://huggingface.co/docs/huggingface_hub)  
- [Transformers para Visão Computacional](https://huggingface.co/docs/transformers/tasks/image_classification)  
- [Modelo DETR (Facebook)](https://huggingface.co/facebook/detr-resnet-50)  
- [Modelo ViT (Google)](https://huggingface.co/google/vit-base-patch16-224)  
- Organização do material com apoio do **ChatGPT**  

---

## Sobre o repositório
Este repositório foi criado como **material de apoio didático** para aulas de Visão Computacional, destacando como utilizar modelos do Hugging Face em exemplos práticos no Colab.
