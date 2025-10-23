# Progetto starter NODE+TYPESCRIPT

## Guida per creare questo progetto

1. Creare cartella del progetto
2. Aprire la cartella del progetto in VS Code
3. Aprire terminale in VC Code
4. Generare il file **package.json**
    ```bash
    npm init -y
    ```
5. Creare a mano la cartella **src**
6. Installare le dipendenze per Typescript
    ```bash
    npm install --save-dev typescript ts-node
    ```
7. Creare il file di configurazione di Typescript **tsconfig.json**
   ```bash
    npx tsc --init
    ```
8. Modificare il file **tsconfig.json**
    ```json
    {  
        "compilerOptions": {
            // File Layout
            "rootDir": "./src",
            "outDir": "./dist"
        }
    }
    ```
9. Modificare **package.json** creando gli scripts
    ```json
    {  
        "scripts": {
            "start": "ts-node ./src/app.ts",
            "build": "tsc"
        },
    }
    ```
10. "Compilare" il progetto
    ```bash
    npm run build
    ```

11. Eseguire il progetto
    ```bash
    npm start
    ```

12. Aggiungere il file **.gitignore**
