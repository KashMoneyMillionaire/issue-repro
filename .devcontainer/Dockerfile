FROM mcr.microsoft.com/vscode/devcontainers/dotnet:8.0

# Update path for dotnet tools and dapr
ENV PATH="${PATH}:/root/.dotnet/tools"
ENV PATH="${PATH}:/home/vscode/.dapr/bin"

# install tools and workloads
RUN dotnet tool install -g Nuke.GlobalTool
RUN dotnet workload update
RUN dotnet workload install aspire
