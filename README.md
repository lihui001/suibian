# suibian
	double ach[134];

	for (int i = 1; i < 68; i++)
	{
		int j = 67 + i;

		if (i == 0)
		{
			ach[j] = 427;
			ach[i] = 512;
		}
		else
		{
			ach[i] = 427 + 1.0 * rand() / RAND_MAX * (512 - 427);
			ach[j] = 903.1 - ach[i];
			if (ach[i] < ach[j])
			{
				swap(ach[i], ach[j]);
			}


			cout << ach[i] << endl;

		}
		for (int i = 0; i < 67; i++) {
			int j = 67 + i;
			for (int m = 0; m < 67 - i; m++)

			{
				swap(ach[i], ach[i + 1]);
				swap(ach[j], ach[j + 1]);
			}
		}
		for (int i = 0; i < 68; i++) {
			cout << ach[i] << endl;
		}
		for (int i = 0; i < 67; i++) {
			int j = 67 + i;
			cout << ach[j] << endl;
		}
	}
