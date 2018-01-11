FROM vitr/casperjs

WORKDIR /app

ADD https://gist.githubusercontent.com/lbalmaceda/3cef267b6bed563d5009a1ca851bac87/raw/ca629d7aa6cdd68b52e87b3cfa3f7f7a809dd297/webapp-test.js tests.js

CMD casperjs test tests.js --fail-fast --initial-url=http://app:3000