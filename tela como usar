import 'package:flutter/material.dart';

class ComoUsarPage extends StatelessWidget {
  const ComoUsarPage({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    final width = MediaQuery.of(context).size.width;

    return Scaffold(
      backgroundColor: Colors.black,
      appBar: AppBar(
        backgroundColor: Colors.black,
        elevation: 0,
        title: const Text(
          'Como usar',
          style: TextStyle(color: Colors.white),
        ),
        centerTitle: true,
        iconTheme: const IconThemeData(color: Colors.white),
      ),
      body: SingleChildScrollView(
        padding: const EdgeInsets.all(20),
        child: Column(
          children: [
            // Logo
            Image.asset(
              'assets/IMG_6624.jpeg',
              width: width * 0.6,
              height: 120,
              fit: BoxFit.contain,
            ),
            const SizedBox(height: 30),

            const _InfoCard(
              emoji: '📌',
              title: 'Adicionar treino',
              text:
                  'Cadastre seus treinos com nome, repetições e carga para cada exercício.',
            ),
            const _InfoCard(
              emoji: '📊',
              title: 'Acompanhar o progresso',
              text:
                  'Veja sua evolução com gráficos semanais e históricos de treino.',
            ),
            const _InfoCard(
              emoji: '⚙️',
              title: 'Alterar dados',
              text:
                  'Atualize suas informações pessoais e metas de desempenho.',
            ),
            const _InfoCard(
              emoji: '💡',
              title: 'Dicas importantes',
              text:
                  'Registre seus treinos com frequência e mantenha sua disciplina. A consistência gera resultados!',
            ),

            const SizedBox(height: 30),
            const Text(
              '💪 SUPERE. EVOLUA. Com o NØSHAPE.',
              textAlign: TextAlign.center,
              style: TextStyle(
                fontStyle: FontStyle.italic,
                fontSize: 15,
                color: Colors.white70,
              ),
            ),
            const SizedBox(height: 20),
          ],
        ),
      ),
    );
  }
}

class _InfoCard extends StatelessWidget {
  final String emoji;
  final String title;
  final String text;

  const _InfoCard({
    required this.emoji,
    required this.title,
    required this.text,
  });

  @override
  Widget build(BuildContext context) {
    return Container(
      width: double.infinity,
      margin: const EdgeInsets.only(bottom: 16),
      padding: const EdgeInsets.all(16),
      decoration: BoxDecoration(
        color: const Color(0xFF1A1A1A),
        borderRadius: BorderRadius.circular(12),
        boxShadow: const [
          BoxShadow(
            color: Colors.black45,
            blurRadius: 4,
            offset: Offset(0, 2),
          )
        ],
      ),
      child: Column(
        crossAxisAlignment: CrossAxisAlignment.start,
        children: [
          Text(
            '$emoji $title',
            style: const TextStyle(
              fontSize: 18,
              fontWeight: FontWeight.bold,
              color: Colors.white,
            ),
          ),
          const SizedBox(height: 6),
          Text(
            text,
            style: const TextStyle(
              fontSize: 15,
              color: Colors.white70,
            ),
          ),
        ],
      ),
    );
  }
}
