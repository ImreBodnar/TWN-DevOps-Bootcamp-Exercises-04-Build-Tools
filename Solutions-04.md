# Solutions for Exercises-04-Build-Tools

## Exercise 0

```bash
# Navigate to the working directory.
cd Repositories

# Cloning.
git clone https://gitlab.com/twn-devops-bootcamp/latest/04-build-tools/build-tools-exercises.git

# Deleting .git folder.
rm -rf build-tools-exercises/.git

# Renaming the folder, because I want to save it to my GitHub repository with a different name.
mv build-tools-exercises TWN-DevOps-Bootcamp-Exercises-04-Build-Tools
cd TWN-DevOps-Bootcamp-Exercises-04-Build-Tools

git init
git status

# Commit & push.
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/ImreBodnar/TWN-DevOps-Bootcamp-Exercises-04-Build-Tools.git
git push -u origin main
```

## Exercise 1

```bash
# Navigate to the working directory.
cd Repositories/TWN-DevOps-Bootcamp-Exercises-04-Build-Tools

# Install gradle.
sudo apt update
sudo apt install gradle

# Try to build.
gradle build
```

## Exercise 2

```bash
# Navigate to the working directory.
cd Repositories/TWN-DevOps-Bootcamp-Exercises-04-Build-Tools

# After I fixed the bug in AppTest.java.
# I need to set JAVA_HOME to Java17 because some incompatibility problems.
export JAVA_HOME=/usr/lib/jvm/java-17-openjdk-amd64
./gradlew test
```

## Exercise 3

```bash
# Navigate to the working directory.
cd Repositories/TWN-DevOps-Bootcamp-Exercises-04-Build-Tools

export JAVA_HOME=/usr/lib/jvm/java-17-openjdk-amd64
./gradlew clean build
```

## Exercise 4

```bash
# Navigate to the working directory.
cd Repositories/TWN-DevOps-Bootcamp-Exercises-04-Build-Tools

export JAVA_HOME=/usr/lib/jvm/java-17-openjdk-amd64
java -jar ./build/libs/build-tools-exercises-1.0-SNAPSHOT.jar
```

## Exercises 5

```bash
# Navigate to the working directory.
cd Repositories/TWN-DevOps-Bootcamp-Exercises-04-Build-Tools

# After I added the given code to log the 2 parameters.
export JAVA_HOME=/usr/lib/jvm/java-17-openjdk-amd64
./gradlew clean build
java -jar ./build/libs/build-tools-exercises-1.0-SNAPSHOT.jar cat dog
```
