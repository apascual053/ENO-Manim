Instalación de Manim
====================

A día de 16 de febrero de 2025, he entrado a la documentación oficial de Manim Community y ha habido cambios en la forma de instalación.

En ocasiones anteriores, creo que recordar que la instalación se llevaba a cabo a través del gestor de paquetes de Python ``pip``. En consecuencia, es necesario gestionar manualmente las depedencias de ManimCE (Manim *Community Edition*). Ahora, en cambio, parece que se fomenta la instalación a través de un nuevo gestor de paquetes denominado ``uv``.

Instalar ``uv``
---------------

Lo primero que he hecho ha sido instalar ``uv`` directamente a través de su script oficial de instalación.

.. prompt:: bash

	curl -LsSf https://astral.sh/uv/install.sh | sh

La respuesta ha sido la siguiente:

.. code-block:: console

	eno-manim@enomanim-VirtualBox:~$ curl -LsSf https://astral.sh/uv/install.sh | sh
	downloading uv 0.6.0 x86_64-unknown-linux-gnu
	no checksums to verify
	installing to /home/eno-manim/.local/bin
	  uv
	  uvx
	everything's installed!

Instalar TexLive (Distribución de LaTeX)
----------------------------------------

Manim esta orientado a usar la distribución de LaTeX en la construcción de fórmulas y ecuaciones matemáticas. Aunque no es necesaría para el correcto funcionamiento de ManimCE, se recomienda su instalación. Para ello, podemos hacer uso del gestor de paquetes de GNU/Linux ``apt``.

.. prompt:: bash

	sudo apt install texlive-full

.. note::

	No es necesaria la instalación completa de la distribución, se puede realizar instalaciones más ligeras. Sin embargo, si no se tiene un conocimiento profundo sobre el funcionamiento de ManimCE y TexLive, se recomiendo la instalación completa, para evitar errores.