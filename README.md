# 🧠 LangGraph Simple Workflow Example

This repository demonstrates how to build a **basic workflow using** in Python. 

It covers the essential steps: defining state, creating nodes, setting conditional edges, compiling the graph, and invoking the workflow. T

his is ideal for beginners exploring agentic flows and LangGraph-based automation.

## 📌 Key Features

- ✅ **Shared State Management** using `TypedDict`

- 🧩 **Modular Node Definitions** (e.g., `start_play`, `cricket`, `basketball`)

- 🔁 **Conditional Flow Control** with randomized branching

- 🛠️ **LangGraph Integration** for easy workflow visualization and execution

- 🖼️ **Graph Visualization** using Mermaid-compatible PNG output


## 🚀 How It Works:

Define a Shared State Schema using TypedDict.

Create Processing Nodes like start_play, cricket, and basketball.

Introduce Conditional Logic using random_play() to switch between nodes.

Assemble the Workflow with StateGraph, define edges, and compile.

Visualize and Run the graph with sample input.

## 📚 Example Output:

When invoked with:

graph_builder.invoke({"graph_info":"I am Shiva Prasad Naroju, "})

You might see outputs like:

- Start play node has been called
- Cricket node has been called

## 🧰 Requirements:

- Python 3.10+

- langgraph

- langchain

- langchain-core

- langchain-community

- IPython.display

- typing_extensions


## ✨ Sample Visualization:

Graph is rendered using Mermaid syntax and displayed as PNG within the notebook using:

- from IPython.display import Image, display

- display(Image(graph_builder.get_graph().draw_mermaid_png()))

