# Open Data Hub - Highlander project

![ODH+EasyBuild+Lmod](./img/banner.png)

<span style="font-size:larger;">Open Data Hub, enhanced with Easybuild and Lmod, or how to bring thousands of libraries and applications to your data science platform without installation!</span>

On a data science platform like [Open Data Hub](http://opendatahub.io/) or [OpenShift Data Science](https://www.redhat.com/en/technologies/cloud-computing/openshift/openshift-data-science), **Container images**  are **hard to manage** if you want to provide users with **many different libraries or applications**, moreover at **various versions**.

This project leverages [EasyBuild](https://easybuild.io/), [Lmod](https://lmod.readthedocs.io/en/latest/) and shared PVCs to bring thousands of those apps and libraries instantly in your notebook. You now have a **single container image** to manage to provide all of them, in **any combination** you want, at **any version** you want! (Therefore the name of the project, "There can be only one…​")

!!! note "WIP, beware..."

    This project is a work in progress to properly refactor the initial code, which is meanwhile still available in different repos, [here](https://github.com/guimou/odh-highlander), [here](https://github.com/guimou/s2i-lmod-notebook) and [here](https://github.com/guimou/jupyter-lmod)
