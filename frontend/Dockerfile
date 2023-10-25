# FROM node:20-slim

# RUN mkdir -p /workspace/frontend/my-app 
# WORKDIR /workspace/frontend/my-app
# # WORKDIR /workspace

# COPY --chown=node:node my-app/package.json my-app/yarn.lock ./

# RUN yarn install

# RUN chown -R node:node /workspace

# COPY --chown=node:node . .

# USER node


# ###########################################
# FROM node:20-slim

# RUN mkdir -p /workspace/frontend/my-app
# WORKDIR /workspace/frontend/my-app

# # USER node

# # COPY my-app/package.json my-app/yarn.lock ./
# COPY --chown=node:node my-app/package.json my-app/yarn.lock ./

# RUN yarn install

# COPY --chown=node:node . .

# RUN chown -R node:node /workspace
# # RUN chmod -R 755 /workspace
# USER node


###########################################
FROM node:20-slim

RUN mkdir -p /workspace/frontend/my-app
WORKDIR /workspace/frontend/my-app

COPY my-app/package.json my-app/yarn.lock ./

RUN yarn install

COPY . .