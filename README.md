# Distance Metrics and K-Nearest Neighbors

An introduction to the distance metrics that power similarity-based machine learning, and to the k-nearest neighbors (KNN) algorithm built on top of them. You start by computing distances by hand in Python, then train KNN with scikit-learn, and finally implement the algorithm from scratch to understand how it works internally.

## Learning Objectives

By the end of this repository, you should be able to:

- Explain and compute the Euclidean, Manhattan, and Minkowski distance metrics.
- Write a general distance function in Python with a tunable norm.
- Train and tune a KNN classifier with scikit-learn.
- Implement the KNN algorithm from scratch and compare it to the scikit-learn version.

## Learning Path

Work through the notebooks in order. Each topic pairs a lesson with a hands-on exercise:

| File / Folder | Description |
|---|---|
| [**1 - Distance Metrics in Python**](1_distance_metric_python.ipynb) | How Euclidean, Manhattan, and Minkowski distances are calculated. |
| [**2 - Distance Metric Exercise**](2_distance_metric_exercise.ipynb) | Write your own `distance()` function with a configurable norm. |
| [**3 - KNN with scikit-learn**](3_knn_sklearn.ipynb) | Train and tune a KNN classifier on a toy dataset. |
| [**4 - KNN Exercise**](4_knn_exercise.ipynb) | Apply KNN to the iris dataset to predict the species. |
| [**5 - KNN from Scratch**](5_knn_from_scratch.ipynb) | Build your own KNN classifier and check it against scikit-learn. |

### Additional Folders and Files

| File / Folder | Description |
|---|---|
| [**Data**](data/) | The iris dataset used in the exercises. |
| [**Assets**](assets/) | Images used in the notebooks. |
| [**Solutions**](solutions/) | Reference solutions. |
| [**pyproject.toml**](pyproject.toml) | Project configuration and dependencies. |
| [**uv.lock**](uv.lock) | Dependency lock file. |

## Setup

> [!NOTE]
> Throughout these steps, text in angle brackets like `<repo-name>` is a
> **placeholder**. Replace it, including the `< >` brackets, with your own
> value. For example, `cd <repo-name>` becomes `cd ds-distance-metrics-knn`.

### 1. Create the Repository from the Template

Click **Use this template** on GitHub.

When creating the repository:

- Set yourself as the **Owner**
- Choose a repository name
- Disable **Include all branches**
- Click **Create repository**

> [!IMPORTANT]
> If you are working in pairs or groups, only **one person** should complete this step.

---

### 2. Add Collaborators (Pairs/Groups Only)

If working with teammates:

1. Open the repository on GitHub
2. Go to **Settings → Collaborators**
3. Add your teammates as collaborators
4. Share the repository link with your team

Teammates should accept the invitation before continuing.

---

### 3. Clone the Repository

Copy the SSH URL from the **Code** button on GitHub, then run:

```bash
git clone <copied-ssh-url>
```

The copied SSH URL will look like `git@github.com:<your-username>/<repo-name>.git`.

---

### 4. Move into the Project Folder and Install Dependencies

This installs all dependencies and creates a virtual environment in `.venv/`.

```bash
cd <repo-name>
uv sync
```

---

### 5. Open the Notebooks

> [!NOTE]
> Make sure you open VS Code from the project root so it automatically detects the environment created by `uv sync`.

Launch VS Code in the project root folder:

```bash
code .
```

Then open a notebook and select the Python environment created by `uv sync` as the kernel.

## References & Further Reading

- [**Scikit-learn: Nearest Neighbors**](https://scikit-learn.org/stable/modules/neighbors.html): The user guide for neighbors-based learning, including KNN.
- [**Scikit-learn: KNeighborsClassifier**](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html): API reference for the classifier and its hyperparameters.
- [**Scikit-learn: Nearest Neighbors Classification example**](https://scikit-learn.org/stable/auto_examples/neighbors/plot_classification.html): A worked example showing how the `weights` parameter shapes decision boundaries.
- [**SciPy: Distance computations**](https://docs.scipy.org/doc/scipy/reference/spatial.distance.html): Reference for the distance metrics available in `scipy.spatial.distance`.
- [**Minkowski distance**](https://en.wikipedia.org/wiki/Minkowski_distance): The generalisation that has Euclidean and Manhattan as special cases.
