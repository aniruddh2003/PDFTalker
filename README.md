# PDFTalker

**PDFTalker** is a Next.js application that allows users to convert PDF files into audio format, offering a seamless experience for transforming written content into an audible form. This project leverages modern technologies like Pinecone DB, PostgreSQL, and the Gemini SDK to provide efficient PDF processing, embedding, and storage.

## Features

- **PDF to Audio Conversion**: Users can upload PDF files and convert them into speech.
- **Vectorization**: Utilizes Pinecone DB for efficient PDF vectorization and retrieval.
- **Embeddings**: Employs Gemini SDK for generating and managing PDF embeddings.
- **Authentication**: Integrated user authentication for secure access and file management.
- **Cloud Storage**: Amazon AWS SDK for securely storing and retrieving PDF and audio files.

## Technologies Used

- **[Next.js](https://nextjs.org/)**: The React framework used to build the web interface.
- **Pinecone DB**: Used for vectorization to handle PDF content efficiently.
- **PostgreSQL**: A robust relational database used for storing metadata, user info, and embeddings.
- **Gemini SDK**: Utilized for generating embeddings to help with the conversion process.
- **Amazon AWS SDK**: Handles file storage on AWS (PDF files and their corresponding audio).
- **Authentication**: Implemented for secure user sessions and managing their files.

## Getting Started

Follow these instructions to get a local copy of the project up and running.

### Prerequisites

Ensure you have the following installed:

- Node.js v16 or higher
- PostgreSQL
- Pinecone DB account
- AWS account with access keys and S3 bucket
- Gemini SDK setup

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/pdftalker.git
    cd pdftalker
    ```

2. Install dependencies:
    ```bash
    npm install
    ```

3. Set up environment variables:
   Create a `.env.local` file in the root directory with the following keys:
    ```bash
    NEXT_PUBLIC_PINECONE_API_KEY=your-pinecone-api-key
    DATABASE_URL=postgres://user:password@localhost:5432/pdftalker
    AWS_ACCESS_KEY_ID=your-aws-access-key
    AWS_SECRET_ACCESS_KEY=your-aws-secret-key
    S3_BUCKET_NAME=your-s3-bucket-name
    GEMINI_API_KEY=your-gemini-api-key
    ```

4. Set up the PostgreSQL database:
    ```bash
    npx prisma migrate dev
    ```

5. Start the development server:
    ```bash
    npm run dev
    ```

6. Open [http://localhost:3000](http://localhost:3000) in your browser to view the app.

### Deployment

This project can be deployed to any platform that supports Next.js, such as Vercel or AWS Amplify. Ensure that the environment variables are set appropriately during deployment.

## Usage

1. **Login** or **Sign Up** to access the platform.
2. Upload your PDF file.
3. Wait for the vectorization and embedding processes to complete.
4. The file will be converted into audio format, which you can download or play directly.

## Contributing

If you want to contribute to this project:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Make your changes.
4. Push the changes (`git push origin feature/your-feature`).
5. Create a pull request.

## License

This project is licensed under the MIT License.

## Contact

For any issues or inquiries, reach out to **[bandyopadhyayaniruddha2@gmail.com]**.
