# Task Description:

## Google Cloud Environment Setup

Before beginning development, set up your workspace on the Google Cloud Platform (GCP).

- Create a new GCP Project.
- Enable the **Vertex AI API**.
- **Important**: We strongly recommend creating a **new Google account** to set up the GCP environment. This allows you to utilize the standard **$300 free credit** provided by Google, ensuring you do not incur any personal costs during this test.

## Agent Configuration & Inputs

Build an agent using **Vertex AI** (You can use any other tool if you want) capable of interpreting natural inputs. The system should allow the user to define the dimensions of a square event space and specify the number of attendees. For the purpose of this challenge, your agent must be able to handle scenarios specifically for small groups (3 to 4 people).

## Generative Room Design

The agent must **generate a visual design** of the room layout.

- Instead of simply plotting points on a graph, the agent should utilize the capabilities of Vertex AI (e.g., using **Gemini** for logic/prompting and **Imagen** for visualization) to create a synthetic image.
- The image must reflect the specific constraints: the correct number of people, the correct furniture layout, and the atmosphere described in your logic.

## Budget Estimation

The agent must calculate and output a preliminary budget for the event setup. You have the freedom to define the cost logic (e.g., furniture, decoration, or space rental costs), but the final output should be a structured financial estimate derived from the space size and the number of people.

## Contextual Image Retrieval

An idea that could maybe help in the Agent's response is enhancing the agent's capabilities by integrating a search mechanism. With this, the system should analyze the generated layout and automatically fetch relevant images from the internet that serve as real-world visual examples of the proposed distribution (e.g., seating charts or small meeting setups).

---

**Bonus: Neurosymbolic Integration (Optional)**

As an extra, demonstrate a Neurosymbolic AI approach. This involves combining symbolic reasoning (using logic to enforce strict rules, such as safety boundaries or geometric constraints) with neural networks (for the generative or unstructured aspects of the task).

**Example**

To help you visualize the expected outcome, here is an example of how the agent should behave inside the notebook:

- **Input**: "I need to organize a relaxed brainstorming session for 4 people in a 6x6 meter room. Please design the space and give me a budget."

- **Output**:

  1. **Strategy Logic**: The agent prints a text explanation (e.g., "Detected 4 people in a 36m² space. Recommending a circular seating arrangement to foster collaboration.").
  2. **Generated Design**: [The Notebook displays a unique, AI-generated image showing a room with comfortable seating for 4 people arranged in a circle].
  3. **Budget**: A printed table showing the estimated cost for 4 lounge chairs, 1 coffee table, and lighting.

**Presentation**

If you want to show us what you did, you can choose to use a jupyter notebook or google colab to output the results from the Agent. Alternatively, you can also work together and coordinate to deploy a small application with a frontend to chat with the Agent.

As we told you, all this is optional, you are not required to do this but it would help with the work you will be doing during your internship.