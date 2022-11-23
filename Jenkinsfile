pipline{
    agent any
    stages{
        stage('Setup Python Virtual ENV')
            {
                steps{
                    sh '''
                    chmod +x envsetup.sh
                    ./envsetup.sh
                    '''
                }
            }
        stage('Gunicorn setup')
            {
                steps{
                    sh '''
                    chmod +x gunicorn.sh
                    ./gunicorn.sh
                    '''
                }
            }
        stage('Nginx setup')
            {
                steps{
                    sh '''
                    chmod +x nginx.sh
                    ./nginx.sh
                    '''
                }
            }
            

    }
}