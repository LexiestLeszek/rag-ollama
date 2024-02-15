# rag-ollama

This is a Gradio-powered web application that allows users to search for academic papers on [arXiv](https://arxiv.org/) and ask questions about them. It uses natural language processing techniques to provide answers based on the content of the papers.

## Features

- Search for academic papers on arXiv.
- Ask questions about the content of the papers.
- Get answers generated by a language model.

## Installation

Install Gradio and other required packages using pip:

```bash
pip install gradio arxiv-dl langchain langchain-community
```

## Usage

Run the application with the following command:

```bash
python gradio_app.py
```

After starting the application, visit `http://localhost:7860` in your web browser to interact with the application. You can enter a search query and a question related to the papers returned by the query.

## Sharing the Application

If you want to share the application publicly, modify the `launch()` call in `app.py` to include `share=True`:

```python
iface.launch(share=True)
```

Running the application with `share=True` will generate a public URL that you can share with others.

## Security Considerations

When sharing your Gradio app, be aware that users will have access to temporary files created by Gradio and files allowed via the `allowed_paths` parameter in `launch()`. Ensure that sensitive information is not exposed through your application and consider adding authentication if necessary.

## Contributing

Contributions to are welcome! Please feel free to submit pull requests or report issues.

## License

this RAG app is licensed under the Apache License  2.0. See the LICENSE file for details.
