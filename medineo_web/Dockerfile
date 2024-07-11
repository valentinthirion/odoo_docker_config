FROM odoo:15.0
USER root
RUN rm -vf /var/lib/apt/lists/*
RUN python3 -m pip install pip
COPY ./medineo_web_content/addons/odoo_web_server/requirements.txt /opt/app/requirements.txt
WORKDIR /opt/app
RUN pip3 install -r requirements.txt
USER odoo