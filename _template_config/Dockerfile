FROM odoo:17.0
USER root
RUN rm -vf /var/lib/apt/lists/*
RUN python3 -m pip install pip
COPY ./_template_content/addons/PROJECT_REPO/requirements.txt /opt/app/requirements.txt
WORKDIR /opt/app
RUN pip3 install -r requirements.txt
USER odoo