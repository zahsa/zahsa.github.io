{% for link in site.data.navigation.main %} {% if link.right %} {{ link.title }} {% else %} {{ link.title }} {% endif %} {% endfor %}
